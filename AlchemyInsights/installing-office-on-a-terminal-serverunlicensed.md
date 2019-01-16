---
title: Cài đặt office trên một máy chủ đầu cuối - không có giấy phép
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28320802"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="5ddfe-102">Cài đặt Office trên một máy chủ đầu cuối</span><span class="sxs-lookup"><span data-stu-id="5ddfe-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="5ddfe-103">Để triển khai Office 365 ProPlus trên một máy chủ Windows bằng cách sử dụng dịch vụ máy tính để bàn từ xa (RDS), tên cũ là dịch vụ đầu cuối:</span><span class="sxs-lookup"><span data-stu-id="5ddfe-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="5ddfe-p101">Bạn phải có một kế hoạch Office 365 bao gồm Office 365 ProPlus, chẳng hạn như Office 365 Enterprise E3 hoặc doanh nghiệp E5. Các gói Office 365 Business và Office 365 doanh nghiệp bảo hiểm không bao gồm Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="5ddfe-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="5ddfe-106">Bạn cần cho phép [dùng chung máy tính kích hoạt](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="5ddfe-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="5ddfe-107">Nếu bạn muốn cài đặt Office 365 ProPlus trên RDS từ cổng Office 365, \*\* *sử dụng thiết lập cài đặt mặc định* \*\*, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="5ddfe-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="5ddfe-p102">Kiểm tra những gì kế hoạch Office 365 bạn có. [Tìm hiểu làm thế nào](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="5ddfe-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>
    
2. <span data-ttu-id="5ddfe-p103">Nếu cần thiết, chuyển sang một khác nhau Office 365 có kế hoạch. [Tìm hiểu làm thế nào](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="5ddfe-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>
    
3. <span data-ttu-id="5ddfe-p104">Nếu văn phòng đã được cài đặt trên máy chủ RDS sử dụng bất kỳ kế hoạch nào khác của Office 365, gỡ bỏ cài đặt nó. Ví dụ, bằng cách vào Control Panel \> gỡ bỏ cài đặt một chương trình. Gỡ cài đặt bằng cách sử dụng [Microsoft hỗ trợ và phục hồi chương trình hỗ trợ](https://aka.ms/SARA-OfficeUninstall-Alchemy) nếu bạn đang chạy vào các vấn đề.</span><span class="sxs-lookup"><span data-stu-id="5ddfe-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="5ddfe-115">Trên máy chủ RDS, đăng nhập vào cổng Office 365 với tài khoản quản trị của bạn và [cài đặt Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="5ddfe-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="5ddfe-116">Sau khi văn phòng được cài đặt, \*\* *không mở hoặc đăng nhập* \*\* cho bất kỳ ứng dụng văn phòng.</span><span class="sxs-lookup"><span data-stu-id="5ddfe-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="5ddfe-117">Trên máy chủ RDS, cho phép dùng chung máy tính kích hoạt bằng cách chỉnh sửa đăng ký bằng cách làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="5ddfe-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="5ddfe-p105">Nhấp chuột phải vào nút Windows trong thấp hơn ở góc bên trái của màn hình của bạn và chọn Run. Trong các mở hộp, loại **regedit**, và sau đó chọn OK.</span><span class="sxs-lookup"><span data-stu-id="5ddfe-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="5ddfe-120">Chọn có khi được nhắc để cho phép trình biên tập Registry để thay đổi thiết bị của bạn.</span><span class="sxs-lookup"><span data-stu-id="5ddfe-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="5ddfe-121">Trong Registry Editor, thêm một chuỗi giá trị của **SharedComputerLicensing** với một thiết lập 1 dưới HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="5ddfe-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="5ddfe-122">Trên máy chủ RDS, \*\* *đăng nhập như là một người sử dụng cuối cùng* \*\* và [xác minh rằng dùng chung máy tính kích hoạt được kích hoạt cho Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="5ddfe-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="5ddfe-123">Để biết thêm chi tiết về điều kiện tiên quyết, hướng dẫn cài đặt và hướng dẫn cài đặt tùy chỉnh bằng cách sử dụng công cụ triển khai văn phòng, hãy xem [Triển khai Office 365 ProPlus bằng cách sử dụng dịch vụ máy tính để bàn từ xa](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="5ddfe-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="5ddfe-124">Để sửa chữa các lỗi liên quan đến dùng chung máy tính kích hoạt, hãy xem [khắc phục sự cố với máy tính được chia sẻ kích hoạt cho Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="5ddfe-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

