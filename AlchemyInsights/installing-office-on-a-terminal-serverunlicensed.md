---
title: Cài đặt Office trên máy chủ đầu cuối-không có giấy phép
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508650"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="ab27d-102">Cài đặt Office trên máy chủ đầu cuối</span><span class="sxs-lookup"><span data-stu-id="ab27d-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="ab27d-103">Để triển khai Microsoft 365 ứng dụng dành cho doanh nghiệp trên Windows Server sử dụng dịch vụ máy tính để bàn từ xa (RDS), trước đây có tên dịch vụ đầu cuối:</span><span class="sxs-lookup"><span data-stu-id="ab27d-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="ab27d-104">Bạn phải đăng ký Microsoft 365 bao gồm Microsoft 365 ứng dụng dành cho doanh nghiệp, chẳng hạn như Office 365 Enterprise E3 hoặc Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="ab27d-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="ab27d-105">Các ứng dụng Microsoft 365 dành cho doanh nghiệp và Microsoft 365 ứng dụng dành cho doanh nghiệp Premium gói không bao gồm Microsoft 365 ứng dụng dành cho doanh nghiệp.</span><span class="sxs-lookup"><span data-stu-id="ab27d-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="ab27d-106">Bạn cần bật [kích hoạt máy tính dùng chung](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="ab27d-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="ab27d-107">Nếu bạn muốn cài đặt Microsoft 365 Apps dành cho doanh nghiệp trên RDS từ Trung tâm quản trị Microsoft 365, sử dụng ***cài đặt mặc định***, sử dụng các bước sau.</span><span class="sxs-lookup"><span data-stu-id="ab27d-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="ab27d-108">Bạn cũng có thể tải xuống và chạy [Microsoft support và Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) để cài đặt Microsoft 365 Apps dành cho doanh nghiệp ở chế độ kích hoạt máy tính dùng chung.</span><span class="sxs-lookup"><span data-stu-id="ab27d-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="ab27d-109">Kiểm tra những gì Microsoft 365 đăng ký bạn có.</span><span class="sxs-lookup"><span data-stu-id="ab27d-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="ab27d-110">Tìm hiểu cách</span><span class="sxs-lookup"><span data-stu-id="ab27d-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="ab27d-111">Nếu cần, chuyển sang đăng ký Microsoft 365 khác.</span><span class="sxs-lookup"><span data-stu-id="ab27d-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="ab27d-112">Tìm hiểu cách</span><span class="sxs-lookup"><span data-stu-id="ab27d-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="ab27d-113">Nếu Office đã được cài đặt trên máy chủ RDS sử dụng bất kỳ đăng ký Microsoft 365 khác, dỡ cài đặt.</span><span class="sxs-lookup"><span data-stu-id="ab27d-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="ab27d-114">Ví dụ: bằng cách đi tới Pa-nen điều khiển \> gỡ cài đặt chương trình.</span><span class="sxs-lookup"><span data-stu-id="ab27d-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="ab27d-115">Dỡ cài đặt bằng cách sử dụng [Microsoft support và phục hồi](https://aka.ms/SARA-OfficeUninstall-Alchemy) hỗ trợ nếu bạn đang chạy vào vấn đề.</span><span class="sxs-lookup"><span data-stu-id="ab27d-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="ab27d-116">Trên máy chủ RDS, đăng nhập vào Trung tâm quản trị Microsoft 365 với tài khoản quản trị viên của bạn và [cài đặt microsoft 365 Apps dành cho doanh nghiệp](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="ab27d-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="ab27d-117">Sau khi Office được cài đặt, ***không mở hoặc đăng nhập*** vào bất kỳ ứng dụng Office.</span><span class="sxs-lookup"><span data-stu-id="ab27d-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="ab27d-118">Trên máy chủ RDS, cho phép kích hoạt máy tính được chia sẻ bằng việc chỉnh sửa sổ đăng ký bằng các bước sau:</span><span class="sxs-lookup"><span data-stu-id="ab27d-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="ab27d-119">Bấm chuột phải vào nút Windows ở góc dưới bên trái của màn hình và chọn chạy.</span><span class="sxs-lookup"><span data-stu-id="ab27d-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="ab27d-120">Trong ô mở, gõ **regedit**, và sau đó chọn OK.</span><span class="sxs-lookup"><span data-stu-id="ab27d-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="ab27d-121">Chọn có khi được nhắc để cho phép Registry Editor thay đổi thiết bị của bạn.</span><span class="sxs-lookup"><span data-stu-id="ab27d-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="ab27d-122">Trong Registry Editor, thêm một giá trị chuỗi **Sharedcomputerlicensing** với thiết đặt 1 trong HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="ab27d-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="ab27d-123">Trên máy chủ RDS, ***đăng nhập như người dùng cuối*** và [xác minh rằng kích hoạt chia sẻ máy tính được kích hoạt cho Microsoft 365 ứng dụng dành cho doanh nghiệp](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="ab27d-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="ab27d-124">Để biết thêm chi tiết về điều kiện tiên quyết, hướng dẫn thiết lập và hướng dẫn cài đặt tuỳ chỉnh bằng cách sử dụng công cụ triển khai Office, hãy xem [triển khai Microsoft 365 ứng dụng dành cho doanh nghiệp bằng cách sử dụng dịch vụ máy tính để bàn từ xa](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="ab27d-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="ab27d-125">Để khắc phục lỗi liên quan đến kích hoạt máy tính dùng chung, hãy xem [khắc phục sự cố với kích hoạt máy tính dùng chung cho Microsoft 365 ứng dụng dành cho doanh nghiệp](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="ab27d-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  