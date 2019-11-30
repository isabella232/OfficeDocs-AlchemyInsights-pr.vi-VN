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
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628264"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="373c7-102">Sửa chữa các ứng dụng Office "chúng tôi không thể kết nối ngay bây giờ" thông báo</span><span class="sxs-lookup"><span data-stu-id="373c7-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="373c7-103">Nếu bạn nhận được thông báo này, hãy thử như sau:</span><span class="sxs-lookup"><span data-stu-id="373c7-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="373c7-104">Kiểm tra tường lửa, phần mềm chống vi-rút và cài đặt proxy để xác nhận rằng chúng không chặn truy cập Internet vào các ứng dụng Office.</span><span class="sxs-lookup"><span data-stu-id="373c7-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="373c7-105">Xem [văn phòng 365 URL và dải địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="373c7-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="373c7-106">Đi để **bắt đầu** > **chạy**, và sau đó gõ **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="373c7-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="373c7-107">Đảm bảo rằng các dịch vụ sau đang chạy:</span><span class="sxs-lookup"><span data-stu-id="373c7-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="373c7-108">Cài đặt tự động thiết bị kết nối mạng</span><span class="sxs-lookup"><span data-stu-id="373c7-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="373c7-109">Dịch vụ danh sách mạng</span><span class="sxs-lookup"><span data-stu-id="373c7-109">Network List Service</span></span>
    - <span data-ttu-id="373c7-110">Nhận thức về vị trí mạng</span><span class="sxs-lookup"><span data-stu-id="373c7-110">Network Location Awareness</span></span>
    - <span data-ttu-id="373c7-111">Nhật ký sự kiện Windows</span><span class="sxs-lookup"><span data-stu-id="373c7-111">Windows Event Log</span></span>

<span data-ttu-id="373c7-112">Nếu một trong các dịch vụ này không chạy, hãy thử khởi động nó.</span><span class="sxs-lookup"><span data-stu-id="373c7-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="373c7-113">Nếu bạn gặp sự cố khởi động dịch vụ, chạy lệnh sau bằng cách mở dấu nhắc lệnh với quyền nâng cao:</span><span class="sxs-lookup"><span data-stu-id="373c7-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="373c7-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="373c7-114">**sfc /scannow**</span></span>

<span data-ttu-id="373c7-115">Sau khi lệnh này kết thúc, khởi động lại máy tính.</span><span class="sxs-lookup"><span data-stu-id="373c7-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="373c7-116">Để biết thông tin chi tiết, xem ["xin lỗi, chúng tôi không thể kết nối với tài khoản của bạn. Vui lòng thử lại sau "lỗi khi bạn kích hoạt Office từ Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="373c7-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>