---
title: Bị kẹt trong hộp thư đi vì các tệp đính kèm lớn
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241274"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="05e06-102">Khắc phục thông báo bị kẹt trong hộp thư đi</span><span class="sxs-lookup"><span data-stu-id="05e06-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="05e06-103">Chúng tôi khuyên bạn bắt đầu bằng cách chạy kịch bản ["tôi gặp sự cố khi gửi, nhận hoặc tìm thư email"](https://aka.ms/SaRA-OutlookSendReceive) từ công cụ [hỗ trợ của Microsoft và trợ lý phục hồi](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="05e06-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="05e06-104">Khi một thông báo bị kẹt trong hộp thư đi của bạn, nguyên nhân có thể là một phần đính kèm lớn hoặc tùy chọn "gửi ngay lập tức khi kết nối" không được phép.</span><span class="sxs-lookup"><span data-stu-id="05e06-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="05e06-105">**Xóa tệp đính kèm lớn**</span><span class="sxs-lookup"><span data-stu-id="05e06-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="05e06-106">Trong Outlook, chọn **gửi/nhận** > **làm việc ngoại tuyến**.</span><span class="sxs-lookup"><span data-stu-id="05e06-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="05e06-107">Trong ngăn điều hướng, chọn **hộp**thư đi.</span><span class="sxs-lookup"><span data-stu-id="05e06-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="05e06-108">Từ đây, bạn có thể:</span><span class="sxs-lookup"><span data-stu-id="05e06-108">From here, you can:</span></span> 
    - <span data-ttu-id="05e06-109">Xoùa tin nhaén (chọn nó và sau đó chọn **Delete**).</span><span class="sxs-lookup"><span data-stu-id="05e06-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="05e06-110">Kéo thư vào thư mục bản thảo của bạn, bấm đúp để mở nó và xóa phần đính kèm, chọn nó rồi chọn **xóa**).</span><span class="sxs-lookup"><span data-stu-id="05e06-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="05e06-111">Nếu bạn nhận được lỗi cho biết Outlook đang cố truyền thư, đóng Outlook.</span><span class="sxs-lookup"><span data-stu-id="05e06-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="05e06-112">Có thể mất vài phút để thoát ra.</span><span class="sxs-lookup"><span data-stu-id="05e06-112">It may take a few moments to exit.</span></span> <span data-ttu-id="05e06-113">Nếu Outlook không đóng, nhấn Ctrl + Alt + Delete và chọn **khởi động trình quản lý tác vụ**.</span><span class="sxs-lookup"><span data-stu-id="05e06-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="05e06-114">Trong Task Manager, chọn tab **quá trình** , cuộn xuống Outlook. exe, và chọn **kết thúc tiến trình**.</span><span class="sxs-lookup"><span data-stu-id="05e06-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="05e06-115">Sau khi Outlook đóng, khởi động lại và lặp lại bước 2 và 3.</span><span class="sxs-lookup"><span data-stu-id="05e06-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="05e06-116">Sau khi bạn loại bỏ phần đính kèm, bấm **gửi/nhận** > **làm việc gián tuyến** để tiếp tục làm việc trực tuyến.</span><span class="sxs-lookup"><span data-stu-id="05e06-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="05e06-117">Thông báo cũng gặp khó khăn trong hộp thư đi khi bạn bấm vào **gửi**, nhưng bạn không được kết nối.</span><span class="sxs-lookup"><span data-stu-id="05e06-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="05e06-118">Nhấp vào **gửi/nhận** và xem nút **làm việc ngoại tuyến** .</span><span class="sxs-lookup"><span data-stu-id="05e06-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="05e06-119">Nếu màu xanh lam, bạn đã bị ngắt kết nối.</span><span class="sxs-lookup"><span data-stu-id="05e06-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="05e06-120">Nhấp vào nó để kết nối (nút chuyển sang màu trắng) và nhấp vào **gửi tất cả**.</span><span class="sxs-lookup"><span data-stu-id="05e06-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="05e06-121">**Cho phép gửi ngay lập tức khi kết nối**</span><span class="sxs-lookup"><span data-stu-id="05e06-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="05e06-122">Trên tab tệp, bấm vào **tuỳ chọn**.</span><span class="sxs-lookup"><span data-stu-id="05e06-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="05e06-123">Trong hộp thoại Tuỳ chọn Outlook, bấm **nâng cao**.</span><span class="sxs-lookup"><span data-stu-id="05e06-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="05e06-124">Trong phần gửi và nhận, bấm để cho phép **gửi ngay lập tức khi kết nối**.</span><span class="sxs-lookup"><span data-stu-id="05e06-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="05e06-125">Bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="05e06-125">Click **OK**.</span></span>
 
<span data-ttu-id="05e06-126">Để biết chi tiết đầy đủ, xem:</span><span class="sxs-lookup"><span data-stu-id="05e06-126">For full details, see:</span></span>
- [<span data-ttu-id="05e06-127">Video: gửi hoặc xóa một email bị kẹt</span><span class="sxs-lookup"><span data-stu-id="05e06-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="05e06-128">Email ở cặp hộp thư đi cho đến khi bạn tự bắt đầu hoạt động gửi/nhận trong Outlook</span><span class="sxs-lookup"><span data-stu-id="05e06-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
