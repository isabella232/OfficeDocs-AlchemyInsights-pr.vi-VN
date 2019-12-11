---
title: Triển khai Office 365 ProPlus để sử dụng chung trên RDS, Terminal Server, hoặc VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959481"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="ec637-102">Triển khai Office 365 ProPlus để sử dụng chung trên RDS, Terminal Server, hoặc VDI</span><span class="sxs-lookup"><span data-stu-id="ec637-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="ec637-103">Triển khai Office 365 ProPlus sử dụng dịch vụ máy tính để bàn từ xa (RDS), trước đây có tên là dịch vụ đầu cuối:</span><span class="sxs-lookup"><span data-stu-id="ec637-103">To deploy Office 365 ProPlus using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="ec637-104">Bạn phải có Microsoft 365 cho kế hoạch kinh doanh hoặc gói Office 365 bao gồm Office 365 ProPlus, chẳng hạn như Office 365 Enterprise E3 hoặc Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="ec637-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="ec637-105">Các gói Office 365 Business và Office 365 Business Premium không bao gồm Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="ec637-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="ec637-106">Bạn phải kích [hoạt máy tính dùng chung](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="ec637-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="ec637-107">Bạn cũng có thể tải xuống và chạy [Microsoft support và Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) để cài đặt Office 365 ProPlus trong chế độ kích hoạt máy tính dùng chung.</span><span class="sxs-lookup"><span data-stu-id="ec637-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="ec637-108">Để biết thêm thông tin về điều kiện tiên quyết, hướng dẫn thiết lập và hướng dẫn cài đặt tuỳ chỉnh bằng cách sử dụng công cụ triển khai Office, hãy xem [triển khai office 365 ProPlus bằng cách sử dụng dịch vụ máy tính để bàn từ xa](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="ec637-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="ec637-109">Để khắc phục lỗi liên quan đến kích hoạt máy tính dùng chung:</span><span class="sxs-lookup"><span data-stu-id="ec637-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="ec637-110">Xem [khắc phục sự cố với kích hoạt máy tính dùng chung cho Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="ec637-110">See [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="ec637-111">Xem [đặt lại trạng thái kích hoạt Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="ec637-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="ec637-112">Nếu bạn muốn cài đặt Office 365 ProPlus trên RDS từ Trung tâm quản trị Microsoft 365, sử ***dụng cài đặt mặc định***, sử dụng các bước sau:</span><span class="sxs-lookup"><span data-stu-id="ec637-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.  <span data-ttu-id="ec637-113">Kiểm tra những gì Office 365 kế hoạch bạn có.</span><span class="sxs-lookup"><span data-stu-id="ec637-113">Check what Office 365 plan you have.</span></span> <span data-ttu-id="ec637-114">[Tìm hiểu làm thế nào](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="ec637-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="ec637-115">Nếu cần thiết, chuyển sang một gói Office 365 khác.</span><span class="sxs-lookup"><span data-stu-id="ec637-115">If necessary, switch to a different Office 365 plan.</span></span> <span data-ttu-id="ec637-116">[Tìm hiểu làm thế nào](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="ec637-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="ec637-117">Nếu Office đã được cài đặt trên máy chủ RDS sử dụng bất kỳ kế hoạch Office 365 khác, dỡ cài đặt.</span><span class="sxs-lookup"><span data-stu-id="ec637-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="ec637-118">Ví dụ, bằng cách đi tới >  **bảng điều khiển\*\*\*\*gỡ bỏ cài đặt một chương trình**.</span><span class="sxs-lookup"><span data-stu-id="ec637-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="ec637-119">Dỡ cài đặt bằng cách sử dụng [Microsoft support và phục hồi](https://aka.ms/SARA-OfficeUninstall-Alchemy) hỗ trợ nếu bạn đang chạy vào vấn đề.</span><span class="sxs-lookup"><span data-stu-id="ec637-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="ec637-120">Trên máy chủ RDS, đăng nhập vào Trung tâm quản trị Microsoft 365 với tài khoản quản trị viên của bạn và [cài đặt Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="ec637-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="ec637-121">Sau khi Office được cài đặt, ***không mở hoặc đăng nhập*** vào bất kỳ ứng dụng Office.</span><span class="sxs-lookup"><span data-stu-id="ec637-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="ec637-122">Trên máy chủ RDS, cho phép kích hoạt máy tính được chia sẻ bằng việc chỉnh sửa sổ đăng ký bằng các bước sau:</span><span class="sxs-lookup"><span data-stu-id="ec637-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="ec637-123">Bấm chuột phải vào nút Windows ở góc dưới bên trái của màn hình và chọn **chạy**.</span><span class="sxs-lookup"><span data-stu-id="ec637-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="ec637-124">Trong ô mở, gõ **regedit**, và sau đó chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="ec637-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="ec637-125">Chọn **có** khi được nhắc để cho phép Registry Editor thay đổi thiết bị của bạn.</span><span class="sxs-lookup"><span data-stu-id="ec637-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="ec637-126">Trong Registry Editor, thêm một giá trị chuỗi **Sharedcomputerlicensing** với thiết đặt 1 trong HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="ec637-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="ec637-127">Trên máy chủ RDS, ***đăng nhập là người dùng cuối*** và [xác minh rằng kích hoạt máy tính dùng chung được kích hoạt cho Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="ec637-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

