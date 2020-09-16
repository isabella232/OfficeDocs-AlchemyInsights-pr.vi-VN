---
title: Khắc phục sự cố ứng dụng Microsoft 365 rất tiếc, chúng tôi có thông báo vấn đề máy chủ tạm thời
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758267"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="55fd5-102">Sửa lỗi ứng dụng Microsoft 365 "rất tiếc, chúng tôi đang gặp phải sự cố máy chủ tạm thời"</span><span class="sxs-lookup"><span data-stu-id="55fd5-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="55fd5-103">Nếu bạn nhận được thông báo này, hãy thử làm như sau:</span><span class="sxs-lookup"><span data-stu-id="55fd5-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="55fd5-104">Kiểm tra tường lửa, phần mềm chống vi-rút và thiết đặt proxy để xác nhận rằng họ không chặn truy nhập Internet vào các ứng dụng Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="55fd5-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="55fd5-105">Xem [dải URL và dải địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="55fd5-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="55fd5-106">Đi đến **bắt đầu**  >  **chạy**, rồi nhập **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="55fd5-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="55fd5-107">Hãy đảm bảo rằng các dịch vụ sau đây đều đang chạy:</span><span class="sxs-lookup"><span data-stu-id="55fd5-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="55fd5-108">Thiết lập tự động thiết bị kết nối mạng</span><span class="sxs-lookup"><span data-stu-id="55fd5-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="55fd5-109">Dịch vụ danh sách mạng</span><span class="sxs-lookup"><span data-stu-id="55fd5-109">Network List Service</span></span>
    - <span data-ttu-id="55fd5-110">Nâng cao vị trí mạng</span><span class="sxs-lookup"><span data-stu-id="55fd5-110">Network Location Awareness</span></span>
    - <span data-ttu-id="55fd5-111">Nhật ký sự kiện Windows</span><span class="sxs-lookup"><span data-stu-id="55fd5-111">Windows Event Log</span></span>

<span data-ttu-id="55fd5-112">Nếu một trong các dịch vụ này không chạy, hãy thử khởi động ứng dụng này.</span><span class="sxs-lookup"><span data-stu-id="55fd5-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="55fd5-113">Nếu bạn gặp sự cố khi bắt đầu dịch vụ, hãy chạy lệnh sau bằng cách mở dấu nhắc lệnh với các quyền tăng cao:</span><span class="sxs-lookup"><span data-stu-id="55fd5-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="55fd5-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="55fd5-114">**sfc /scannow**</span></span>

<span data-ttu-id="55fd5-115">Sau khi lệnh này kết thúc, hãy khởi động lại máy tính.</span><span class="sxs-lookup"><span data-stu-id="55fd5-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="55fd5-116">Để biết thông tin chi tiết, hãy xem ["xin lỗi, chúng tôi không thể kết nối với tài khoản của bạn. Vui lòng thử lại sau "lỗi" khi bạn kích hoạt](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="55fd5-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>