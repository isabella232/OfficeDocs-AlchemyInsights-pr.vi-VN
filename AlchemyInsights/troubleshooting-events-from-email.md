---
title: Khắc phục sự kiện từ email
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569398"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="3dac5-102">Khắc phục sự kiện từ email</span><span class="sxs-lookup"><span data-stu-id="3dac5-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="3dac5-103">Kiểm tra tính năng được kích hoạt cho hộp thư: **nhận-EventsFromEmailConfiguration <mailbox> -Identity**</span><span class="sxs-lookup"><span data-stu-id="3dac5-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="3dac5-104">Sau đó nhìn vào các ' sự kiện từ email ' Nhật ký **xuất khẩu-Mailboxchẩn Sticlogs <mailbox> -cấu phần timeprofile**</span><span class="sxs-lookup"><span data-stu-id="3dac5-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="3dac5-105">Trong Nhật ký "sự kiện từ email", tìm InternetMessageId phù hợp với mục trong hộp thư.</span><span class="sxs-lookup"><span data-stu-id="3dac5-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="3dac5-106">TrustScore xác định nếu mục được thêm vào hay không.</span><span class="sxs-lookup"><span data-stu-id="3dac5-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="3dac5-107">Sự kiện sẽ chỉ được thêm vào nếu TrustScore = "tin cậy".</span><span class="sxs-lookup"><span data-stu-id="3dac5-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="3dac5-108">TrustScore được xác định bởi SPF, DKIM hoặc dMarc thuộc tính, trong tiêu đề thư.</span><span class="sxs-lookup"><span data-stu-id="3dac5-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="3dac5-109">Để xem các tính này:</span><span class="sxs-lookup"><span data-stu-id="3dac5-109">To view these properties:</span></span>

<span data-ttu-id="3dac5-110">**Máy tính để bàn Outlook**</span><span class="sxs-lookup"><span data-stu-id="3dac5-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="3dac5-111">Mở mục</span><span class="sxs-lookup"><span data-stu-id="3dac5-111">Open the item</span></span>
- <span data-ttu-id="3dac5-112">Tệp-> Properties-> tiêu đề Internet</span><span class="sxs-lookup"><span data-stu-id="3dac5-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="3dac5-113">Hoặc</span><span class="sxs-lookup"><span data-stu-id="3dac5-113">or</span></span>

<span data-ttu-id="3dac5-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="3dac5-114">**MFCMapi**</span></span>

- <span data-ttu-id="3dac5-115">Điều hướng đến mục trong hộp thư đến</span><span class="sxs-lookup"><span data-stu-id="3dac5-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="3dac5-116">Tìm kiếm PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="3dac5-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="3dac5-117">Các tính này được xác định và ghi lại trong quá trình vận chuyển và định tuyến.</span><span class="sxs-lookup"><span data-stu-id="3dac5-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="3dac5-118">Để khắc phục sự cố thêm, bạn có thể cần phải theo dõi hỗ trợ truyền tải về các lỗi trong SPF, DKIM và. hoặc DMARC.</span><span class="sxs-lookup"><span data-stu-id="3dac5-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>