---
title: Tôi nhận quyền truy nhập có điều kiện với thiết bị đã tham gia tên miền
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038108"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="25ed1-102">Tôi nhận quyền truy nhập có điều kiện với thiết bị đã tham gia tên miền</span><span class="sxs-lookup"><span data-stu-id="25ed1-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="25ed1-103">**Công cụ được đề xuất cao**</span><span class="sxs-lookup"><span data-stu-id="25ed1-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="25ed1-104">[Công cụ trình gỡ rối đăng ký thiết bị](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) -công cụ giúp khắc phục sự cố đăng ký thiết bị phổ biến nhất.</span><span class="sxs-lookup"><span data-stu-id="25ed1-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="25ed1-105">Trình [kiểm tra kết nối đăng ký thiết bị](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) -Script giúp đảm bảo rằng thiết bị có thể truy nhập các điểm cuối đăng ký thiết bị bên dưới tài khoản hệ thống.</span><span class="sxs-lookup"><span data-stu-id="25ed1-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="25ed1-106">[Kịch bản dọn dẹp thiết bị AZURE AD](https://github.com/mzmaili/AzureADDeviceCleanup) -tập lệnh cho phép bạn tìm kiếm và quản lý các thiết bị cũ trong môi trường của bạn.</span><span class="sxs-lookup"><span data-stu-id="25ed1-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="25ed1-107">Dưới đây là một số lý do phổ biến tại sao truy nhập có điều kiện có thể không phải là một thiết bị đã gia nhập một tên miền (kết hợp Azure AD).</span><span class="sxs-lookup"><span data-stu-id="25ed1-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="25ed1-108">**Không có AZURE AD PRT trên thiết bị** -bạn cần đảm bảo rằng thiết bị có mã thông báo làm mới của Azure AD (PRT).</span><span class="sxs-lookup"><span data-stu-id="25ed1-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="25ed1-109">Để biết thêm thông tin về PRT, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)này.</span><span class="sxs-lookup"><span data-stu-id="25ed1-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="25ed1-110">Để xác nhận nếu bạn có Azure AD PRT, bạn có thể chạy `dsregcmd/status` lệnh trên thiết bị và xác nhận xem "AzureAdPrt" bằng "có".</span><span class="sxs-lookup"><span data-stu-id="25ed1-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="25ed1-111">Nếu "AzureAdPrt" là "không", hãy kiểm tra như sau:</span><span class="sxs-lookup"><span data-stu-id="25ed1-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="25ed1-112">**Cho dù bạn có môi trường được liên kết với AD FS và không thể truy nhập được từ mạng nhà của người dùng của bạn**: trong trường hợp này, hãy đảm bảo rằng các điểm cuối "usernamemixed" của bạn có thể truy nhập từ Extranet.</span><span class="sxs-lookup"><span data-stu-id="25ed1-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="25ed1-113">Nếu AD FS của bạn nằm phía sau một VPN, hãy đảm bảo rằng người dùng kết nối với VPN và đăng nhập lại vào thiết bị.</span><span class="sxs-lookup"><span data-stu-id="25ed1-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="25ed1-114">Để biết thêm thông tin, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)này.</span><span class="sxs-lookup"><span data-stu-id="25ed1-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="25ed1-115">**Cho dù thiết bị của TPM bị lỗi và do đó không thể xác thực thiết bị**: Hãy kiểm tra "TPM. msc" để xem trạng thái của TPM là "đã sẵn sàng".</span><span class="sxs-lookup"><span data-stu-id="25ed1-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="25ed1-116">Nếu không, `dsregcmd/leave` hãy chạy và để thiết bị gia nhập lại AZURE AD.</span><span class="sxs-lookup"><span data-stu-id="25ed1-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="25ed1-117">Sau đó, hãy thử lại.</span><span class="sxs-lookup"><span data-stu-id="25ed1-117">Then, try again.</span></span> <span data-ttu-id="25ed1-118">Để biết thêm thông tin, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)này.</span><span class="sxs-lookup"><span data-stu-id="25ed1-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="25ed1-119">**Bạn đang sử dụng nhà cung cấp căn cước bên thứ 3, vốn không hỗ trợ giao thức WS-Trust**.</span><span class="sxs-lookup"><span data-stu-id="25ed1-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="25ed1-120">Như được mô tả trong tài liệu của chúng tôi, kết hợp Azure AD được gia nhập vào các thiết bị không thể làm việc trong trường hợp này.</span><span class="sxs-lookup"><span data-stu-id="25ed1-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="25ed1-121">Vui lòng làm việc với nhà cung cấp căn cước của bạn để được hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="25ed1-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="25ed1-122">**Người dùng đang sử dụng trình duyệt Chrome mà không có tài khoản Windows 10** hoặc **Chrome của Office sẽ không tự động sử dụng PRT trên thiết bị đã tham gia hoặc** kết hợp kết hợp-kết hợp với thiết bị được gia nhập: điều này sẽ dẫn đến sự thất bại của bất kỳ thông báo lỗi truy nhập có điều kiện dựa trên thiết bị nào được hiển thị.</span><span class="sxs-lookup"><span data-stu-id="25ed1-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="25ed1-123">Để sử dụng trình duyệt Chrome chính xác, bạn phải cài đặt phần mở rộng "tài khoản Windows 10" hoặc "Office Extension với trình duyệt Chrome của người dùng" thông qua SCCM hoặc InTune.</span><span class="sxs-lookup"><span data-stu-id="25ed1-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="25ed1-124">Để biết thêm thông tin, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)này.</span><span class="sxs-lookup"><span data-stu-id="25ed1-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="25ed1-125">Nếu bạn không thể đẩy phần mở rộng từ xa, hãy thông báo cho người dùng để cài đặt thủ công một trong các phần mở rộng để truy nhập vào các ứng dụng sau quyền truy nhập có điều kiện dựa trên thiết bị.</span><span class="sxs-lookup"><span data-stu-id="25ed1-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="25ed1-126">Để biết thêm thông tin, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)này.</span><span class="sxs-lookup"><span data-stu-id="25ed1-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="25ed1-127">**Thiết bị được kết hợp đúng cách kết hợp AZURE AD đã gia nhập nhưng đã vô tình bị xóa hoặc tắt, do việc đồng bộ thay đổi trong AZURE AD Connect hoặc từ Azure Portal**: nếu điều này xảy ra, đối tượng thiết bị sẽ không còn được nhận diện là thiết bị được gia nhập đầy đủ, mặc dù trạng thái "AzureAdJoined" và</span><span class="sxs-lookup"><span data-stu-id="25ed1-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="25ed1-128">Để khắc phục sự cố này, `dsregcmd/leave` hãy chạy trên các thiết bị bị ảnh hưởng và để họ tái gia nhập AZURE AD.</span><span class="sxs-lookup"><span data-stu-id="25ed1-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="25ed1-129">Để biết thêm thông tin, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)này.</span><span class="sxs-lookup"><span data-stu-id="25ed1-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="25ed1-130">Nếu các thiết bị của bạn đang ở trên Windows 10, 1809 Cập Nhật, với VPN/proxy proxy và xem các vấn đề với "AzureAdPrt" State hoặc ứng dụng bất kỳ với vấn đề SSO (Outlook không kết nối đến hộp thư ngay cả khi bạn đã có PRT), hãy đảm bảo bạn có bản vá này [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) hoặc bản Cập Nhật tích lũy tháng tư [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) để ngăn chặn các</span><span class="sxs-lookup"><span data-stu-id="25ed1-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















