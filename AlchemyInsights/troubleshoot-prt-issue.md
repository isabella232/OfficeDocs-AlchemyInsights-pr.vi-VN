---
title: Khắc phục sự cố PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573906"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="a1572-102">Khắc phục sự cố PRT</span><span class="sxs-lookup"><span data-stu-id="a1572-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="a1572-103">Đối với bất kỳ thiết bị nào để hoàn tất việc nhận đã được xác thực, nó phải được đăng ký đầy đủ và trong trạng thái tốt và có thể thu được mã thông báo làm mới chính (PRT).</span><span class="sxs-lookup"><span data-stu-id="a1572-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="a1572-104">Quy trình tham gia đăng ký kết hợp Azure AD sẽ yêu cầu thiết bị trên mạng công ty.</span><span class="sxs-lookup"><span data-stu-id="a1572-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="a1572-105">Nó cũng hoạt động trên VPN nhưng có một số cẩn thận với điều đó.</span><span class="sxs-lookup"><span data-stu-id="a1572-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="a1572-106">Chúng tôi đã nghe những khách hàng cần trợ giúp khắc phục sự cố về quy trình đăng ký kết hợp Azure.</span><span class="sxs-lookup"><span data-stu-id="a1572-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="a1572-107">Đây là một sự cố về những điều đang xảy ra ' dưới mui xe ' trong quá trình đăng ký.</span><span class="sxs-lookup"><span data-stu-id="a1572-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="a1572-108">**Môi trường xác thực đám mây (sử dụng tính năng đồng bộ hóa băm mật khẩu Azure AD hoặc chuyển qua)**</span><span class="sxs-lookup"><span data-stu-id="a1572-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="a1572-109">Dòng đăng ký này còn được gọi là "đồng bộ gia nhập".</span><span class="sxs-lookup"><span data-stu-id="a1572-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="a1572-110">Windows 10 phát hiện ra một bản ghi SCP khi người dùng đăng nhập vào thiết bị.</span><span class="sxs-lookup"><span data-stu-id="a1572-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="a1572-111">Trước tiên, thiết bị cố gắng truy xuất thông tin đối tượng thuê từ SCP bên máy khách trong sổ đăng ký [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="a1572-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="a1572-112">Để biết thêm thông tin, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)này.</span><span class="sxs-lookup"><span data-stu-id="a1572-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="a1572-113">Nếu không thành công, thiết bị liên lạc với Active Directory tại cơ sở (quảng cáo) để nhận thông tin đối tượng thuê từ điểm kết nối dịch vụ (SCP).</span><span class="sxs-lookup"><span data-stu-id="a1572-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="a1572-114">Để xác nhận SCP, vui lòng tham khảo [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)này.</span><span class="sxs-lookup"><span data-stu-id="a1572-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="a1572-115">Chúng tôi khuyên bạn nên bật SCP trong quảng cáo và chỉ sử dụng SCP bên máy khách để xác thực ban đầu.</span><span class="sxs-lookup"><span data-stu-id="a1572-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="a1572-116">Windows 10 sẽ cố gắng liên lạc với Azure AD bên dưới ngữ cảnh hệ thống để xác thực chính nó với Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a1572-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="a1572-117">Bạn có thể xác nhận liệu thiết bị có thể truy nhập tài nguyên Microsoft bên dưới tài khoản hệ thống bằng cách sử dụng script kết nối đăng ký thiết bị kiểm tra.</span><span class="sxs-lookup"><span data-stu-id="a1572-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="a1572-118">Windows 10 tạo chứng chỉ tự ký và lưu trữ nó bên dưới đối tượng máy tính trong quảng cáo tại cơ sở.</span><span class="sxs-lookup"><span data-stu-id="a1572-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="a1572-119">Điều này yêu cầu phải có đường ngắm cho bộ điều khiển tên miền.</span><span class="sxs-lookup"><span data-stu-id="a1572-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="a1572-120">Đối tượng thiết bị có chứng chỉ được đồng bộ hóa với Azure AD thông qua Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a1572-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="a1572-121">Chu kỳ đồng bộ là mỗi 30 phút theo mặc định, nhưng tùy thuộc vào cấu hình của Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a1572-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="a1572-122">Để biết thêm thông tin, vui lòng tham khảo [tài liệu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)này.</span><span class="sxs-lookup"><span data-stu-id="a1572-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="a1572-123">Ở giai đoạn này, bạn sẽ có thể nhìn thấy thiết bị chủ đề trong trạng thái "đang chờ" bên dưới thanh thiết bị của Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="a1572-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="a1572-124">Tại mục đăng nhập của người dùng tiếp theo vào Windows 10, việc đăng ký sẽ được hoàn thành.</span><span class="sxs-lookup"><span data-stu-id="a1572-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="a1572-125">Nếu bạn đang ở trên VPN và quá trình đăng nhập kết thúc kết nối tên miền, bạn có thể kích hoạt theo cách thủ công:</span><span class="sxs-lookup"><span data-stu-id="a1572-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="a1572-126">Phát hành hàm dsregcmd/join cục bộ trên lời nhắc quản trị hoặc từ xa qua PSExec đến PC của bạn.</span><span class="sxs-lookup"><span data-stu-id="a1572-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="a1572-127">Ví dụ: PsExec-s \\ win10client01 CMD, dsregcmd/join</span><span class="sxs-lookup"><span data-stu-id="a1572-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="a1572-128">Để biết thêm chi tiết về các vấn đề gia nhập kết hợp, hãy xem [khắc phục sự cố thiết bị](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="a1572-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
