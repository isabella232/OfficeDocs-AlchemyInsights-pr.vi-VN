---
title: Vấn đề về kích hoạt-chúng tôi không thể kết nối ngay bây giờ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806464"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="b9ec9-102">Sửa các ứng dụng Microsoft 365 "chúng tôi không thể kết nối ngay bây giờ"</span><span class="sxs-lookup"><span data-stu-id="b9ec9-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="b9ec9-103">Nếu bạn nhận được thông báo này, hãy thử làm như sau:</span><span class="sxs-lookup"><span data-stu-id="b9ec9-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="b9ec9-104">Kiểm tra tường lửa, phần mềm chống vi-rút và thiết đặt proxy để xác nhận rằng họ không chặn truy nhập Internet vào các ứng dụng Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b9ec9-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="b9ec9-105">Xem các [URL và dải địa chỉ IP của Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="b9ec9-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="b9ec9-106">Đi đến **bắt đầu**  >  **chạy**, rồi nhập **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="b9ec9-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="b9ec9-107">Hãy đảm bảo rằng các dịch vụ sau đây đều đang chạy:</span><span class="sxs-lookup"><span data-stu-id="b9ec9-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="b9ec9-108">Thiết lập tự động thiết bị kết nối mạng</span><span class="sxs-lookup"><span data-stu-id="b9ec9-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="b9ec9-109">Dịch vụ danh sách mạng</span><span class="sxs-lookup"><span data-stu-id="b9ec9-109">Network List Service</span></span>
    - <span data-ttu-id="b9ec9-110">Nâng cao vị trí mạng</span><span class="sxs-lookup"><span data-stu-id="b9ec9-110">Network Location Awareness</span></span>
    - <span data-ttu-id="b9ec9-111">Nhật ký sự kiện Windows</span><span class="sxs-lookup"><span data-stu-id="b9ec9-111">Windows Event Log</span></span>

<span data-ttu-id="b9ec9-112">Nếu một trong các dịch vụ này không chạy, hãy thử khởi động ứng dụng này.</span><span class="sxs-lookup"><span data-stu-id="b9ec9-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="b9ec9-113">Nếu bạn gặp sự cố khi bắt đầu dịch vụ, hãy chạy lệnh sau bằng cách mở dấu nhắc lệnh với các quyền tăng cao:</span><span class="sxs-lookup"><span data-stu-id="b9ec9-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="b9ec9-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="b9ec9-114">**sfc /scannow**</span></span>

<span data-ttu-id="b9ec9-115">Sau khi lệnh này kết thúc, hãy khởi động lại máy tính.</span><span class="sxs-lookup"><span data-stu-id="b9ec9-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="b9ec9-116">Để biết thông tin chi tiết, hãy xem ["xin lỗi, chúng tôi không thể kết nối với tài khoản của bạn. Vui lòng thử lại sau "lỗi" khi bạn kích hoạt Office từ Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="b9ec9-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>