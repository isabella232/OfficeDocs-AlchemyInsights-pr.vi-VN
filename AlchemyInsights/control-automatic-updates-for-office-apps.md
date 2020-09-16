---
title: Điều khiển Cập nhật tự động cho các ứng dụng Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747798"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="06242-102">Điều khiển Cập nhật tự động cho các ứng dụng Office</span><span class="sxs-lookup"><span data-stu-id="06242-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="06242-103">Theo mặc định, các bản Cập Nhật cho các ứng dụng Office được tự động tải xuống và áp dụng trong nền mà không có bất kỳ sự can thiệp của người dùng.</span><span class="sxs-lookup"><span data-stu-id="06242-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="06242-104">Tuy nhiên, người quản trị có thể kiểm soát cách áp dụng các bản Cập Nhật bằng cách dùng thiết đặt Cập Nhật Office.</span><span class="sxs-lookup"><span data-stu-id="06242-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="06242-105">Thiết đặt Cập Nhật cho phép người quản trị bật hoặc tắt Cập nhật tự động, Hiển thị hoặc ẩn nút **Cập Nhật ngay** trong Office, đặt thời hạn Cập Nhật và nhiều hơn nữa.</span><span class="sxs-lookup"><span data-stu-id="06242-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="06242-106">Để biết thông tin chi tiết, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="06242-106">For detailed information, see:</span></span>

- [<span data-ttu-id="06242-107">Cấu hình thiết đặt Cập Nhật cho Office</span><span class="sxs-lookup"><span data-stu-id="06242-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="06242-108">Cập nhật tự động cho Office không được bật</span><span class="sxs-lookup"><span data-stu-id="06242-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="06242-109">Xác định cách Cập Nhật Office sau khi cài đặt nó</span><span class="sxs-lookup"><span data-stu-id="06242-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="06242-110">Để xem lại các thiết đặt Cập Nhật hiện có được áp dụng cho máy khách, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="06242-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="06242-111">Mở trình soạn thảo sổ đăng ký bằng cách đi đến **bắt đầu**  >  **chạy**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="06242-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="06242-112">Chuyển đến vị trí sau đây và xem lại các thiết đặt Cập Nhật Office:</span><span class="sxs-lookup"><span data-stu-id="06242-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="06242-113">một.</span><span class="sxs-lookup"><span data-stu-id="06242-113">a.</span></span> <span data-ttu-id="06242-114">HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="06242-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="06242-115">b.</span><span class="sxs-lookup"><span data-stu-id="06242-115">b.</span></span> <span data-ttu-id="06242-116">Gỡ cài đặt cấu hình</span><span class="sxs-lookup"><span data-stu-id="06242-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="06242-117">**Ghi chú**  Nếu khóa officemgmtcom được đặt, bạn có thể thấy thông báo "bản Cập Nhật được quản lý bởi người quản **Office**trị hệ thống của bạn" trong các  >  **Account**  >  **bản Cập Nhật**tài khoản Office.</span><span class="sxs-lookup"><span data-stu-id="06242-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="06242-118">Để biết thêm thông tin, hãy xem [quản lý các bản Cập Nhật cho ứng dụng microsoft 365 với Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="06242-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  