---
title: Vấn đề kích hoạt-chúng tôi không thể kết nối ngay bây giờ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581897"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="1bfe7-102">Sửa chữa các ứng dụng Microsoft 365 "chúng tôi không thể kết nối ngay bây giờ" tin nhắn</span><span class="sxs-lookup"><span data-stu-id="1bfe7-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="1bfe7-103">Nếu bạn nhận được thông báo này, hãy thử như sau:</span><span class="sxs-lookup"><span data-stu-id="1bfe7-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="1bfe7-104">Kiểm tra tường lửa, phần mềm chống vi-rút và cài đặt proxy để xác nhận rằng chúng không chặn truy cập Internet tới các ứng dụng Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1bfe7-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="1bfe7-105">Xem [các URL của Microsoft và các phạm vi địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="1bfe7-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="1bfe7-106">Đi tới **bắt đầu**  >  **chạy**, và sau đó gõ **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="1bfe7-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="1bfe7-107">Đảm bảo rằng các dịch vụ sau đang chạy:</span><span class="sxs-lookup"><span data-stu-id="1bfe7-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="1bfe7-108">Cài đặt tự động thiết bị kết nối mạng</span><span class="sxs-lookup"><span data-stu-id="1bfe7-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="1bfe7-109">Dịch vụ danh sách mạng</span><span class="sxs-lookup"><span data-stu-id="1bfe7-109">Network List Service</span></span>
    - <span data-ttu-id="1bfe7-110">Nhận thức về vị trí mạng</span><span class="sxs-lookup"><span data-stu-id="1bfe7-110">Network Location Awareness</span></span>
    - <span data-ttu-id="1bfe7-111">Nhật ký sự kiện Windows</span><span class="sxs-lookup"><span data-stu-id="1bfe7-111">Windows Event Log</span></span>

<span data-ttu-id="1bfe7-112">Nếu một trong các dịch vụ này không chạy, hãy thử khởi động nó.</span><span class="sxs-lookup"><span data-stu-id="1bfe7-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="1bfe7-113">Nếu bạn gặp sự cố khởi động dịch vụ, chạy lệnh sau bằng cách mở dấu nhắc lệnh với quyền nâng cao:</span><span class="sxs-lookup"><span data-stu-id="1bfe7-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="1bfe7-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="1bfe7-114">**sfc /scannow**</span></span>

<span data-ttu-id="1bfe7-115">Sau khi lệnh này kết thúc, khởi động lại máy tính.</span><span class="sxs-lookup"><span data-stu-id="1bfe7-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="1bfe7-116">Để biết thông tin chi tiết, xem ["xin lỗi, chúng tôi không thể kết nối với tài khoản của bạn. Vui lòng thử lại sau "lỗi khi bạn kích hoạt Office từ Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="1bfe7-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>