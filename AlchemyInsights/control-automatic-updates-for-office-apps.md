---
title: Kiểm soát Cập nhật tự động cho các ứng dụng Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439930"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="8db78-102">Kiểm soát Cập nhật tự động cho các ứng dụng Office</span><span class="sxs-lookup"><span data-stu-id="8db78-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="8db78-103">Theo mặc định, bản Cập Nhật cho ứng dụng Office được tải xuống tự động và áp dụng trong nền mà không cần bất kỳ sự can thiệp của người dùng.</span><span class="sxs-lookup"><span data-stu-id="8db78-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="8db78-104">Tuy nhiên, quản trị viên có thể kiểm soát cách áp dụng bản Cập Nhật bằng cách sử dụng cài đặt Office Update.</span><span class="sxs-lookup"><span data-stu-id="8db78-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="8db78-105">Cài đặt Cập Nhật cho phép quản trị viên bật hoặc tắt Cập nhật tự động, Hiển thị hoặc ẩn nút **Cập Nhật ngay** trong Office, đặt Cập Nhật thời hạn và hơn thế nữa.</span><span class="sxs-lookup"><span data-stu-id="8db78-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="8db78-106">Để biết thông tin chi tiết, xem:</span><span class="sxs-lookup"><span data-stu-id="8db78-106">For detailed information, see:</span></span>

- [<span data-ttu-id="8db78-107">Cấu hình cài đặt bản Cập Nhật cho Office</span><span class="sxs-lookup"><span data-stu-id="8db78-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="8db78-108">Cập nhật tự động cho Office không được kích hoạt</span><span class="sxs-lookup"><span data-stu-id="8db78-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="8db78-109">Xác định cách Office được cập nhật sau khi cài đặt</span><span class="sxs-lookup"><span data-stu-id="8db78-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="8db78-110">Để đánh giá cài đặt bản Cập Nhật hiện tại được áp dụng cho máy khách, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="8db78-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="8db78-111">Mở Registry Editor bằng đi để **bắt đầu**  >  **chạy**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="8db78-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="8db78-112">Chuyển sang vị trí sau và đánh giá cài đặt Cập Nhật Office:</span><span class="sxs-lookup"><span data-stu-id="8db78-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="8db78-113">A.</span><span class="sxs-lookup"><span data-stu-id="8db78-113">a.</span></span> <span data-ttu-id="8db78-114">HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="8db78-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="8db78-115">B.</span><span class="sxs-lookup"><span data-stu-id="8db78-115">b.</span></span> <span data-ttu-id="8db78-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="8db78-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="8db78-117">**Lưu ý**  Nếu khoá officemgmtcom được thiết lập, bạn có thể thấy thông báo "Cập Nhật được quản lý bởi quản trị hệ thống của bạn **" trong văn phòng**  >  **tài khoản**Office  >  **Cập Nhật**.</span><span class="sxs-lookup"><span data-stu-id="8db78-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="8db78-118">Để biết thêm thông tin, xem [quản lý bản Cập Nhật cho microsoft 365 ứng dụng với Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="8db78-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  