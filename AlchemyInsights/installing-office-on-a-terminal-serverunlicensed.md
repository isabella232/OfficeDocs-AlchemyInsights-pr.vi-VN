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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37205431"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="2dcbc-102">Cài đặt Office trên máy chủ đầu cuối</span><span class="sxs-lookup"><span data-stu-id="2dcbc-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="2dcbc-103">Để triển khai Office 365 ProPlus trên Windows Server sử dụng dịch vụ máy tính để bàn từ xa (RDS), trước đây có tên dịch vụ đầu cuối:</span><span class="sxs-lookup"><span data-stu-id="2dcbc-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="2dcbc-104">Bạn phải có một gói Office 365 bao gồm Office 365 ProPlus, chẳng hạn như Office 365 Enterprise E3 hoặc Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="2dcbc-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="2dcbc-105">Các gói Office 365 Business và Office 365 Business Premium không bao gồm Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="2dcbc-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="2dcbc-106">Bạn cần bật [kích hoạt máy tính dùng chung](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="2dcbc-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="2dcbc-107">Nếu bạn muốn cài đặt Office 365 ProPlus trên RDS từ Trung tâm quản trị Microsoft 365, sử ***dụng cài đặt mặc định***, sử dụng các bước sau.</span><span class="sxs-lookup"><span data-stu-id="2dcbc-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="2dcbc-108">Bạn cũng có thể tải xuống và chạy [Microsoft support và Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) để cài đặt Office 365 ProPlus trong chế độ kích hoạt máy tính dùng chung.</span><span class="sxs-lookup"><span data-stu-id="2dcbc-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="2dcbc-109">Kiểm tra những gì Office 365 kế hoạch bạn có.</span><span class="sxs-lookup"><span data-stu-id="2dcbc-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="2dcbc-110">Tìm hiểu cách</span><span class="sxs-lookup"><span data-stu-id="2dcbc-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="2dcbc-111">Nếu cần thiết, chuyển sang một gói Office 365 khác.</span><span class="sxs-lookup"><span data-stu-id="2dcbc-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="2dcbc-112">Tìm hiểu cách</span><span class="sxs-lookup"><span data-stu-id="2dcbc-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="2dcbc-113">Nếu Office đã được cài đặt trên máy chủ RDS sử dụng bất kỳ kế hoạch Office 365 khác, dỡ cài đặt.</span><span class="sxs-lookup"><span data-stu-id="2dcbc-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="2dcbc-114">Ví dụ: bằng cách đi tới Pa \> -nen điều khiển gỡ cài đặt chương trình.</span><span class="sxs-lookup"><span data-stu-id="2dcbc-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="2dcbc-115">Dỡ cài đặt bằng cách sử dụng [Microsoft support và phục hồi](https://aka.ms/SARA-OfficeUninstall-Alchemy) hỗ trợ nếu bạn đang chạy vào vấn đề.</span><span class="sxs-lookup"><span data-stu-id="2dcbc-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="2dcbc-116">Trên máy chủ RDS, đăng nhập vào Trung tâm quản trị Microsoft 365 với tài khoản quản trị viên của bạn và [cài đặt Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="2dcbc-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="2dcbc-117">Sau khi Office được cài đặt, ***không mở hoặc đăng nhập*** vào bất kỳ ứng dụng Office.</span><span class="sxs-lookup"><span data-stu-id="2dcbc-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="2dcbc-118">Trên máy chủ RDS, cho phép kích hoạt máy tính được chia sẻ bằng việc chỉnh sửa sổ đăng ký bằng các bước sau:</span><span class="sxs-lookup"><span data-stu-id="2dcbc-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="2dcbc-119">Bấm chuột phải vào nút Windows ở góc dưới bên trái của màn hình và chọn chạy.</span><span class="sxs-lookup"><span data-stu-id="2dcbc-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="2dcbc-120">Trong ô mở, gõ **regedit**, và sau đó chọn OK.</span><span class="sxs-lookup"><span data-stu-id="2dcbc-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="2dcbc-121">Chọn có khi được nhắc để cho phép Registry Editor thay đổi thiết bị của bạn.</span><span class="sxs-lookup"><span data-stu-id="2dcbc-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="2dcbc-122">Trong Registry Editor, thêm một giá trị chuỗi **Sharedcomputerlicensing** với thiết đặt 1 trong HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="2dcbc-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="2dcbc-123">Trên máy chủ RDS, ***đăng nhập là người dùng cuối*** và [xác minh rằng kích hoạt máy tính dùng chung được kích hoạt cho Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="2dcbc-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="2dcbc-124">Để biết thêm chi tiết về điều kiện tiên quyết, hướng dẫn thiết lập và hướng dẫn cài đặt tuỳ chỉnh bằng cách sử dụng công cụ triển khai Office, hãy xem [triển khai Office 365 ProPlus bằng cách sử dụng dịch vụ máy tính để bàn từ xa](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="2dcbc-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="2dcbc-125">Để khắc phục lỗi liên quan đến kích hoạt máy tính dùng chung, vui lòng xem [khắc phục sự cố với kích hoạt máy tính dùng chung cho Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="2dcbc-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  