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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716194"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="2af47-102">Sửa chữa các ứng dụng Office "chúng tôi không thể kết nối ngay bây giờ" thông báo</span><span class="sxs-lookup"><span data-stu-id="2af47-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="2af47-103">Nếu bạn nhận được thông báo này, hãy thử như sau:</span><span class="sxs-lookup"><span data-stu-id="2af47-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="2af47-104">Kiểm tra tường lửa, phần mềm chống vi-rút và cài đặt proxy để xác nhận rằng chúng không chặn truy cập Internet vào các ứng dụng Office.</span><span class="sxs-lookup"><span data-stu-id="2af47-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="2af47-105">Xem [các URL của Microsoft và các phạm vi địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="2af47-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="2af47-106">Đi để **bắt đầu** > **chạy**, và sau đó gõ **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="2af47-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="2af47-107">Đảm bảo rằng các dịch vụ sau đang chạy:</span><span class="sxs-lookup"><span data-stu-id="2af47-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="2af47-108">Cài đặt tự động thiết bị kết nối mạng</span><span class="sxs-lookup"><span data-stu-id="2af47-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="2af47-109">Dịch vụ danh sách mạng</span><span class="sxs-lookup"><span data-stu-id="2af47-109">Network List Service</span></span>
    - <span data-ttu-id="2af47-110">Nhận thức về vị trí mạng</span><span class="sxs-lookup"><span data-stu-id="2af47-110">Network Location Awareness</span></span>
    - <span data-ttu-id="2af47-111">Nhật ký sự kiện Windows</span><span class="sxs-lookup"><span data-stu-id="2af47-111">Windows Event Log</span></span>

<span data-ttu-id="2af47-112">Nếu một trong các dịch vụ này không chạy, hãy thử khởi động nó.</span><span class="sxs-lookup"><span data-stu-id="2af47-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="2af47-113">Nếu bạn gặp sự cố khởi động dịch vụ, chạy lệnh sau bằng cách mở dấu nhắc lệnh với quyền nâng cao:</span><span class="sxs-lookup"><span data-stu-id="2af47-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="2af47-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="2af47-114">**sfc /scannow**</span></span>

<span data-ttu-id="2af47-115">Sau khi lệnh này kết thúc, khởi động lại máy tính.</span><span class="sxs-lookup"><span data-stu-id="2af47-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="2af47-116">Để biết thông tin chi tiết, xem ["xin lỗi, chúng tôi không thể kết nối với tài khoản của bạn. Vui lòng thử lại sau "lỗi khi bạn kích hoạt Office từ Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="2af47-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>