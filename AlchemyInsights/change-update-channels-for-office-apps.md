---
title: Thay đổi các kênh Cập Nhật cho các ứng dụng Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 43a3cdefe5a9bc1726984a3195dce7aaea08d892
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786875"
---
# <a name="change-update-channels-for-office-apps"></a><span data-ttu-id="9cc97-102">Thay đổi các kênh Cập Nhật cho các ứng dụng Office</span><span class="sxs-lookup"><span data-stu-id="9cc97-102">Change update channels for Office apps</span></span>

<span data-ttu-id="9cc97-103">Đối với các bản cài đặt Office mới, hãy dùng thiết đặt tải xuống phần mềm Office để chọn kênh Cập Nhật mong muốn, sau đó cài đặt (hoặc cài đặt lại) các ứng dụng Office.</span><span class="sxs-lookup"><span data-stu-id="9cc97-103">For new Office installations, use Office Software Download Settings to select the desired update channel, and then install (or re-install) Office apps.</span></span> <span data-ttu-id="9cc97-104">Để biết thêm thông tin, hãy xem [quản lý các thiết đặt tải xuống phần mềm trong Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span><span class="sxs-lookup"><span data-stu-id="9cc97-104">For more info, see [Manage software download settings in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span></span> 

<span data-ttu-id="9cc97-105">**Ghi chú** Kênh Cập Nhật được chọn bằng cách sử dụng thiết đặt tải xuống phần mềm Office áp dụng cho tất cả người dùng thực hiện cài đặt mới bằng cách dùng cổng thông tin O365.</span><span class="sxs-lookup"><span data-stu-id="9cc97-105">**Note** The update channel selected using the Office Software Download Settings applies to all users performing new installations using the O365 portal.</span></span> <span data-ttu-id="9cc97-106">Để biết thêm thông tin, hãy xem [tải xuống và cài đặt hoặc cài đặt lại Microsoft 365 hoặc Office 2019 trên PC hoặc máy Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span><span class="sxs-lookup"><span data-stu-id="9cc97-106">For more info, see [Download and install or reinstall Microsoft 365 or Office 2019 on a PC or Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span></span>   

<span data-ttu-id="9cc97-107">Đối với các bản cài đặt Office hiện có, hãy sử dụng công cụ triển khai Office (ODT) để chuyển sang kênh Cập Nhật khác:</span><span class="sxs-lookup"><span data-stu-id="9cc97-107">For existing Office installations, use the Office Deployment Tool (ODT) to switch to a different update channel:</span></span>  

1. <span data-ttu-id="9cc97-108">Tải xuống phiên bản mới nhất của công cụ triển khai Office (setup.exe) từ [Trung tâm tải xuống của Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="9cc97-108">Download the latest version of the Office Deployment Tool (setup.exe) from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
2. <span data-ttu-id="9cc97-109">Xác định tên kênh mà bạn muốn chuyển sang.</span><span class="sxs-lookup"><span data-stu-id="9cc97-109">Identify the name of the channel that you want to switch to.</span></span> <span data-ttu-id="9cc97-110">Để biết thêm thông tin, hãy xem [tùy chọn cấu hình cho công cụ triển khai Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span><span class="sxs-lookup"><span data-stu-id="9cc97-110">For more info, see [Configuration options for the Office Deployment Tool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span></span>
3. <span data-ttu-id="9cc97-111">Tạo một tệp XML cấu hình xác định tên kênh thích hợp, ví dụ, update.xml.</span><span class="sxs-lookup"><span data-stu-id="9cc97-111">Create a configuration XML file specifying the appropriate channel name, for example, update.xml.</span></span>  

`<Configuration>`<br>
`<Updates Channel="Current"/>`<br>
`</Configuration>`<br>

4. <span data-ttu-id="9cc97-112">Từ dấu nhắc lệnh nâng cao, hãy chuyển đến vị trí thư mục nơi setup.exe cư trú và chạy lệnh sau đây:</span><span class="sxs-lookup"><span data-stu-id="9cc97-112">From an elevated command prompt, switch to the folder location where setup.exe resides and run the following command:</span></span>  
    <span data-ttu-id="9cc97-113">một.</span><span class="sxs-lookup"><span data-stu-id="9cc97-113">a.</span></span> <span data-ttu-id="9cc97-114">setup.exe/Configure update.xml</span><span class="sxs-lookup"><span data-stu-id="9cc97-114">setup.exe /configure update.xml</span></span>
5. <span data-ttu-id="9cc97-115">Khởi động một ứng dụng Office (chẳng hạn như Excel), **File**rồi chọn  >  **tài khoản**tệp.</span><span class="sxs-lookup"><span data-stu-id="9cc97-115">Start an Office application (such as Excel), and then select **File** > **Account**.</span></span> <span data-ttu-id="9cc97-116">Trong phần thông tin sản phẩm, chọn Cập Nhật **tùy chọn cập**Nhật  >  **ngay bây giờ**.</span><span class="sxs-lookup"><span data-stu-id="9cc97-116">In the Product Information section, select **Update Options** > **Update Now**.</span></span>

<span data-ttu-id="9cc97-117">Để biết thêm thông tin, hãy xem [làm thế nào để chuyển các kênh Cập Nhật cho các ứng dụng Office hiện có](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span><span class="sxs-lookup"><span data-stu-id="9cc97-117">For more information, see [How to switch update channels for existing Office Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span></span> 

<span data-ttu-id="9cc97-118">Để chuyển đổi các kênh Cập Nhật cho một nhóm người dùng được chọn hoặc bằng cách sử dụng trình quản lý cấu hình (SCCM), cấu hình thiết đặt kênh Cập Nhật bằng GPO.</span><span class="sxs-lookup"><span data-stu-id="9cc97-118">For switching update channels for a selected group of users or by using Configuration Manager (SCCM), configure the Update Channel setting using GPO.</span></span> <span data-ttu-id="9cc97-119">Để biết thêm thông tin, hãy xem [tổng quan về các kênh Cập Nhật cho ứng dụng Microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span><span class="sxs-lookup"><span data-stu-id="9cc97-119">For more info, see [Overview of update channels for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span></span> <span data-ttu-id="9cc97-120">Để biết chi tiết, hãy xem [làm thế nào để quản lý các kênh Office 365 ProPlus cho CNTT ưu](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) và [quản lý các bản Cập Nhật cho ứng dụng Microsoft 365 với Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="9cc97-120">For details, see [How to manage Office 365 ProPlus Channels for IT Pros](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) and [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span></span>