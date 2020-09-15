---
title: Cài đặt Office trên máy chủ kết nối-không được cấp phép
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663139"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="bc7fb-102">Cài đặt Office trên máy chủ đầu cuối</span><span class="sxs-lookup"><span data-stu-id="bc7fb-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="bc7fb-103">Đối với triển khai ứng dụng Microsoft 365 cho doanh nghiệp trên Windows Server bằng cách dùng dịch vụ Remote trên máy tính (RDS), trước đây có tên là dịch vụ Terminal:</span><span class="sxs-lookup"><span data-stu-id="bc7fb-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="bc7fb-104">Bạn phải có đăng ký Microsoft 365 bao gồm các ứng dụng Microsoft 365 cho doanh nghiệp, chẳng hạn như Office 365 Enterprise E3 hoặc Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="bc7fb-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="bc7fb-105">Ứng dụng Microsoft 365 dành cho doanh nghiệp và Microsoft 365 dành cho các gói Business Premium sẽ không bao gồm các ứng dụng Microsoft 365 cho doanh nghiệp.</span><span class="sxs-lookup"><span data-stu-id="bc7fb-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="bc7fb-106">Bạn cần cho phép [kích hoạt máy tính được chia sẻ](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="bc7fb-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="bc7fb-107">Nếu bạn muốn cài đặt các ứng dụng Microsoft 365 cho doanh nghiệp trên RDS từ Trung tâm quản trị Microsoft 365, sử dụng các ***thiết đặt cài đặt mặc định***, hãy làm theo các bước sau đây.</span><span class="sxs-lookup"><span data-stu-id="bc7fb-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="bc7fb-108">Bạn cũng có thể tải xuống và chạy công cụ [Trợ giúp phục hồi và hỗ trợ của Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) để cài đặt ứng dụng Microsoft 365 cho doanh nghiệp trong chế độ kích hoạt máy tính dùng chung.</span><span class="sxs-lookup"><span data-stu-id="bc7fb-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="bc7fb-109">Kiểm tra xem bạn có thuê bao Microsoft 365 nào.</span><span class="sxs-lookup"><span data-stu-id="bc7fb-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="bc7fb-110">Tìm hiểu cách thức</span><span class="sxs-lookup"><span data-stu-id="bc7fb-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="bc7fb-111">Nếu cần, hãy chuyển sang đăng ký khác của Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bc7fb-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="bc7fb-112">Tìm hiểu cách thức</span><span class="sxs-lookup"><span data-stu-id="bc7fb-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="bc7fb-113">Nếu Office đã được cài đặt trên máy chủ RDS bằng bất kỳ thuê bao nào khác của Microsoft 365, hãy dỡ cài đặt nó.</span><span class="sxs-lookup"><span data-stu-id="bc7fb-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="bc7fb-114">Ví dụ, bằng cách đi tới Pa-nen điều khiển để \> gỡ cài đặt một chương trình.</span><span class="sxs-lookup"><span data-stu-id="bc7fb-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="bc7fb-115">Gỡ cài đặt bằng cách sử dụng trợ [lý phục hồi và hỗ trợ của Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) nếu bạn đang gặp phải vấn đề.</span><span class="sxs-lookup"><span data-stu-id="bc7fb-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="bc7fb-116">Trên máy chủ RDS, hãy đăng nhập vào Trung tâm quản trị Microsoft 365 với tài khoản người quản trị của bạn và [cài đặt các ứng dụng microsoft 365 cho doanh nghiệp](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="bc7fb-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="bc7fb-117">Sau khi đã cài đặt Office, ***Đừng mở hoặc đăng nhập*** vào bất kỳ ứng dụng Office nào.</span><span class="sxs-lookup"><span data-stu-id="bc7fb-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="bc7fb-118">Trên máy chủ RDS, cho phép kích hoạt máy tính được chia sẻ bằng cách sửa sổ đăng ký bằng cách thực hiện theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="bc7fb-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="bc7fb-119">Bấm chuột phải vào nút Windows ở góc dưới bên trái màn hình của bạn, rồi chọn chạy.</span><span class="sxs-lookup"><span data-stu-id="bc7fb-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="bc7fb-120">Trong hộp mở, nhập **regedit**, rồi chọn OK.</span><span class="sxs-lookup"><span data-stu-id="bc7fb-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="bc7fb-121">Chọn có khi được nhắc để cho phép trình soạn thảo sổ đăng ký thực hiện thay đổi đối với thiết bị của bạn.</span><span class="sxs-lookup"><span data-stu-id="bc7fb-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="bc7fb-122">Trong trình soạn thảo sổ đăng ký, hãy thêm một giá trị chuỗi của **Sharedcomputercấp phép** với một thiết đặt của 1 dưới HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \ Office\clicktorun\configuration.</span><span class="sxs-lookup"><span data-stu-id="bc7fb-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="bc7fb-123">Trên máy chủ RDS, ***đăng nhập là người dùng cuối*** và [xác minh rằng kích hoạt máy tính được chia sẻ được bật cho các ứng dụng Microsoft 365 dành cho doanh nghiệp](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="bc7fb-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="bc7fb-124">Để biết thêm chi tiết về điều kiện tiên quyết, hướng dẫn thiết lập và hướng dẫn về cài đặt tùy chỉnh bằng cách sử dụng công cụ triển khai Office, vui lòng xem [triển khai ứng dụng Microsoft 365 cho doanh nghiệp bằng cách sử dụng các dịch vụ trên máy tính từ xa](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="bc7fb-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="bc7fb-125">Để khắc phục các lỗi liên quan đến kích hoạt máy tính được chia sẻ, vui lòng xem [khắc phục sự cố với kích hoạt máy tính dùng chung cho các ứng dụng Microsoft 365 dành cho doanh nghiệp](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="bc7fb-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  