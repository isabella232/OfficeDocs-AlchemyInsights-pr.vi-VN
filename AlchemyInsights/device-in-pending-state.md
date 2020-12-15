---
title: Thiết bị trong trạng thái đang chờ xử lý
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679997"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="3d18a-102">Thiết bị trong trạng thái đang chờ xử lý</span><span class="sxs-lookup"><span data-stu-id="3d18a-102">Device in pending state</span></span>

<span data-ttu-id="3d18a-103">**OLSync**</span><span class="sxs-lookup"><span data-stu-id="3d18a-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="3d18a-104">Nếu bạn đang thiết lập đăng ký thiết bị lần đầu tiên, vui lòng đảm bảo rằng bạn đã xem xét việc [giới thiệu về quản lý thiết bị trong Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) sẽ hướng dẫn bạn về cách tải các thiết bị dưới phần điều khiển của Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3d18a-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="3d18a-105">Nếu bạn đang đăng ký thiết bị vào Azure AD trực tiếp và ghi lại chúng vào InTune, bạn sẽ cần phải đảm bảo rằng bạn đã [cấu hình InTune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) và có [cấp phép](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) tại chỗ trước tiên.</span><span class="sxs-lookup"><span data-stu-id="3d18a-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="3d18a-106">Đảm bảo bạn được phép thực hiện các hoạt động trong Azure AD và quảng cáo tại cơ sở.</span><span class="sxs-lookup"><span data-stu-id="3d18a-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="3d18a-107">Chỉ có một người quản trị toàn cầu trong Azure AD có thể quản lý thiết đặt cho việc đăng ký thiết bị.</span><span class="sxs-lookup"><span data-stu-id="3d18a-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="3d18a-108">Ngoài ra, nếu bạn đang thiết lập đăng ký tự động trong Active Directory tại chỗ của bạn, bạn sẽ cần phải là người quản trị của Active Directory và AD FS (nếu có).</span><span class="sxs-lookup"><span data-stu-id="3d18a-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="3d18a-109">Quy trình tham gia đăng ký kết hợp Azure AD sẽ yêu cầu thiết bị trên mạng công ty.</span><span class="sxs-lookup"><span data-stu-id="3d18a-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="3d18a-110">Nó cũng hoạt động trên VPN nhưng có một số cẩn thận với điều đó.</span><span class="sxs-lookup"><span data-stu-id="3d18a-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="3d18a-111">Chúng tôi đã nghe những khách hàng cần trợ giúp khắc phục sự cố về quy trình đăng ký kết hợp Azure.</span><span class="sxs-lookup"><span data-stu-id="3d18a-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="3d18a-112">**Môi trường xác thực đám mây (sử dụng tính năng đồng bộ hóa băm mật khẩu Azure AD hoặc chuyển qua)**</span><span class="sxs-lookup"><span data-stu-id="3d18a-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="3d18a-113">Dòng đăng ký này còn được gọi là "đồng bộ gia nhập".</span><span class="sxs-lookup"><span data-stu-id="3d18a-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="3d18a-114">Dưới đây là một sự cố về những điều sẽ xảy ra trong quá trình đăng ký:</span><span class="sxs-lookup"><span data-stu-id="3d18a-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="3d18a-115">Bản ghi điểm kết nối dịch vụ phát hiện Windows 10 (SCP) khi người dùng đăng nhập vào thiết bị.</span><span class="sxs-lookup"><span data-stu-id="3d18a-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="3d18a-116">Trước tiên, thiết bị cố gắng truy xuất thông tin đối tượng thuê từ SCP bên máy khách trong sổ đăng ký [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="3d18a-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="3d18a-117">Để biết thêm thông tin, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="3d18a-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="3d18a-118">Nếu không thành công, thiết bị liên lạc với Active Directory tại chỗ để nhận thông tin về đối tượng thuê từ SCP.</span><span class="sxs-lookup"><span data-stu-id="3d18a-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="3d18a-119">Để xác nhận SCP, hãy tham khảo [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)này.</span><span class="sxs-lookup"><span data-stu-id="3d18a-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="3d18a-120">Chúng tôi khuyên bạn nên bật SCP trong Active Directory và chỉ sử dụng SCP-Side cho máy khách để xác thực ban đầu.</span><span class="sxs-lookup"><span data-stu-id="3d18a-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="3d18a-121">Windows 10 sẽ cố gắng liên lạc với Azure AD bên dưới ngữ cảnh hệ thống để xác thực chính nó với Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3d18a-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="3d18a-122">Bạn có thể xác nhận liệu thiết bị có thể truy nhập tài nguyên Microsoft bên dưới tài khoản hệ thống bằng cách sử dụng [script kết nối đăng ký thiết bị kiểm tra](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="3d18a-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="3d18a-123">Windows 10 tạo chứng chỉ tự ký và lưu trữ nó bên dưới đối tượng máy tính trong Active Directory tại chỗ.</span><span class="sxs-lookup"><span data-stu-id="3d18a-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="3d18a-124">Điều này yêu cầu phải có đường ngắm cho bộ điều khiển tên miền.</span><span class="sxs-lookup"><span data-stu-id="3d18a-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="3d18a-125">Đối tượng thiết bị có chứng chỉ được đồng bộ hóa với Azure AD thông qua Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="3d18a-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="3d18a-126">Chu kỳ đồng bộ là mỗi 30 phút theo mặc định, nhưng tùy thuộc vào cấu hình của Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="3d18a-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="3d18a-127">Để biết thêm thông tin, hãy tham khảo [tài liệu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)này.</span><span class="sxs-lookup"><span data-stu-id="3d18a-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="3d18a-128">Ở giai đoạn này, bạn sẽ có thể nhìn thấy thiết bị chủ đề trong trạng thái "**đang chờ**" bên dưới thanh thiết bị của Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="3d18a-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="3d18a-129">Tại mục đăng nhập của người dùng tiếp theo vào Windows 10, việc đăng ký sẽ được hoàn thành.</span><span class="sxs-lookup"><span data-stu-id="3d18a-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="3d18a-130">Nếu bạn đang ở trên VPN và đăng xuất/đăng nhập chấm dứt khả năng kết nối tên miền, bạn có thể kích hoạt việc đăng ký theo cách thủ công.</span><span class="sxs-lookup"><span data-stu-id="3d18a-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="3d18a-131">Để thực hiện điều đó:</span><span class="sxs-lookup"><span data-stu-id="3d18a-131">To do that:</span></span>
    >
    > <span data-ttu-id="3d18a-132">Phát hành `dsregcmd /join` lời nhắc người quản trị cục bộ hoặc từ xa qua PSExec sang PC của bạn.</span><span class="sxs-lookup"><span data-stu-id="3d18a-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="3d18a-133">Ví dụ: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="3d18a-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="3d18a-134">Đối với các sự cố phổ biến với đăng ký thiết bị Azure Active Directory, hãy xem [thiết bị câu hỏi thường gặp](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="3d18a-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
