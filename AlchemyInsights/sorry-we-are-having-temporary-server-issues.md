---
title: Sửa chữa các ứng dụng Microsoft 365 xin lỗi, chúng tôi đang gặp sự cố máy chủ tạm thời thông báo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582725"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="af488-102">Sửa chữa các ứng dụng Microsoft 365 "xin lỗi, chúng tôi đang gặp sự cố máy chủ tạm thời" thông báo</span><span class="sxs-lookup"><span data-stu-id="af488-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="af488-103">Nếu bạn nhận được thông báo này, hãy thử như sau:</span><span class="sxs-lookup"><span data-stu-id="af488-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="af488-104">Kiểm tra tường lửa, phần mềm chống vi-rút và cài đặt proxy để xác nhận rằng chúng không chặn truy cập Internet tới các ứng dụng Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="af488-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="af488-105">Xem [URL và phạm vi địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="af488-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="af488-106">Đi tới **bắt đầu**  >  **chạy**, và sau đó gõ **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="af488-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="af488-107">Đảm bảo rằng các dịch vụ sau đang chạy:</span><span class="sxs-lookup"><span data-stu-id="af488-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="af488-108">Cài đặt tự động thiết bị kết nối mạng</span><span class="sxs-lookup"><span data-stu-id="af488-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="af488-109">Dịch vụ danh sách mạng</span><span class="sxs-lookup"><span data-stu-id="af488-109">Network List Service</span></span>
    - <span data-ttu-id="af488-110">Nhận thức về vị trí mạng</span><span class="sxs-lookup"><span data-stu-id="af488-110">Network Location Awareness</span></span>
    - <span data-ttu-id="af488-111">Nhật ký sự kiện Windows</span><span class="sxs-lookup"><span data-stu-id="af488-111">Windows Event Log</span></span>

<span data-ttu-id="af488-112">Nếu một trong các dịch vụ này không chạy, hãy thử khởi động nó.</span><span class="sxs-lookup"><span data-stu-id="af488-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="af488-113">Nếu bạn gặp sự cố khởi động dịch vụ, chạy lệnh sau bằng cách mở dấu nhắc lệnh với quyền nâng cao:</span><span class="sxs-lookup"><span data-stu-id="af488-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="af488-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="af488-114">**sfc /scannow**</span></span>

<span data-ttu-id="af488-115">Sau khi lệnh này kết thúc, khởi động lại máy tính.</span><span class="sxs-lookup"><span data-stu-id="af488-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="af488-116">Để biết thông tin chi tiết, xem ["xin lỗi, chúng tôi không thể kết nối với tài khoản của bạn. Vui lòng thử lại sau "lỗi khi bạn kích hoạt](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="af488-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>