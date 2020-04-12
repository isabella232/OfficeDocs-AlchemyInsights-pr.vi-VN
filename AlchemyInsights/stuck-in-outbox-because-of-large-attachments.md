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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232652"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="07369-102">Khắc phục thông báo bị kẹt trong hộp thư đi</span><span class="sxs-lookup"><span data-stu-id="07369-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="07369-103">Chúng tôi khuyên bạn bắt đầu bằng cách chạy kịch bản ["tôi gặp sự cố khi gửi, nhận hoặc tìm thư email"](https://aka.ms/SaRA-OutlookSendReceive) từ công cụ [Microsoft support và Recovery Assistant](https://diagnostics.office.com/#/) trên máy bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="07369-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="07369-104">Khi một thông báo bị kẹt trong hộp thư đi của bạn, nguyên nhân có thể là một phần đính kèm lớn hoặc tùy chọn "gửi ngay lập tức khi kết nối" không được phép.</span><span class="sxs-lookup"><span data-stu-id="07369-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="07369-105">**Xóa tệp đính kèm lớn**</span><span class="sxs-lookup"><span data-stu-id="07369-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="07369-106">Nhấp vào **gửi/nhận** > **làm việc gián tuyến**.</span><span class="sxs-lookup"><span data-stu-id="07369-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="07369-107">Trong ngăn điều hướng, nhấp vào **hộp**thư đi.</span><span class="sxs-lookup"><span data-stu-id="07369-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="07369-108">Từ đây, bạn có thể:</span><span class="sxs-lookup"><span data-stu-id="07369-108">From here, you can:</span></span> 
    - <span data-ttu-id="07369-109">Xoùa tin nhaén.</span><span class="sxs-lookup"><span data-stu-id="07369-109">Delete the message.</span></span> <span data-ttu-id="07369-110">Chỉ cần chọn nó và nhấp vào **xóa**.</span><span class="sxs-lookup"><span data-stu-id="07369-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="07369-111">Kéo thư vào **thư mục bản thảo**của bạn, bấm đúp vào để mở thư và xóa phần đính kèm (nhấp vào nó và nhấp vào **xóa**).</span><span class="sxs-lookup"><span data-stu-id="07369-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="07369-112">Nếu lỗi cho bạn biết Outlook đang cố gắng truyền thư, đóng Outlook.</span><span class="sxs-lookup"><span data-stu-id="07369-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="07369-113">Có thể mất vài phút để thoát ra.</span><span class="sxs-lookup"><span data-stu-id="07369-113">It may take a few moments to exit.</span></span> <span data-ttu-id="07369-114">Nếu Outlook không đóng, nhấn **Ctrl + Alt + Delete** và bấm **bắt đầu trình quản lý tác vụ**.</span><span class="sxs-lookup"><span data-stu-id="07369-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="07369-115">Trong Task Manager, chọn tab **quá trình** , cuộn xuống Outlook. exe, và bấm **kết thúc tiến trình**.</span><span class="sxs-lookup"><span data-stu-id="07369-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="07369-116">Sau khi Outlook đóng, khởi động lại Outlook và lặp lại bước 2-3.</span><span class="sxs-lookup"><span data-stu-id="07369-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="07369-117">Sau khi bạn loại bỏ các tập tin đính kèm, nhấp vào **gửi/nhận** > **làm việc offline** chọn nút và để tiếp tục làm việc trực tuyến.</span><span class="sxs-lookup"><span data-stu-id="07369-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="07369-118">Thông báo cũng gặp khó khăn trong hộp thư đi khi bạn bấm vào **gửi**, nhưng bạn không được kết nối.</span><span class="sxs-lookup"><span data-stu-id="07369-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="07369-119">Nhấp vào **gửi/nhận** và xem nút **làm việc ngoại tuyến** .</span><span class="sxs-lookup"><span data-stu-id="07369-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="07369-120">Nếu màu xanh lam, bạn đã bị ngắt kết nối.</span><span class="sxs-lookup"><span data-stu-id="07369-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="07369-121">Nhấp vào nó để kết nối (nút chuyển sang màu trắng) và nhấp vào **gửi tất cả**.</span><span class="sxs-lookup"><span data-stu-id="07369-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="07369-122">**Cho phép gửi ngay lập tức khi kết nối**</span><span class="sxs-lookup"><span data-stu-id="07369-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="07369-123">Trên tab tệp, bấm vào **tuỳ chọn**.</span><span class="sxs-lookup"><span data-stu-id="07369-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="07369-124">Trong hộp thoại Tuỳ chọn Outlook, bấm **nâng cao**.</span><span class="sxs-lookup"><span data-stu-id="07369-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="07369-125">Trong phần gửi và nhận, bấm để cho phép **gửi ngay lập tức khi kết nối**.</span><span class="sxs-lookup"><span data-stu-id="07369-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="07369-126">Bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="07369-126">Click **OK**.</span></span>
 
<span data-ttu-id="07369-127">Để biết chi tiết đầy đủ, xem:</span><span class="sxs-lookup"><span data-stu-id="07369-127">For full details, see:</span></span>
- [<span data-ttu-id="07369-128">Video: gửi hoặc xóa một email bị kẹt</span><span class="sxs-lookup"><span data-stu-id="07369-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="07369-129">Email ở cặp hộp thư đi cho đến khi bạn tự bắt đầu hoạt động gửi/nhận trong Outlook</span><span class="sxs-lookup"><span data-stu-id="07369-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
