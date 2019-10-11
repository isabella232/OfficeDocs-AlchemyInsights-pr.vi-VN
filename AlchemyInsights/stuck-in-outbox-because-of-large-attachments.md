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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441327"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="6e490-102">Khắc phục thông báo bị kẹt trong hộp thư đi</span><span class="sxs-lookup"><span data-stu-id="6e490-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="6e490-103">Chúng tôi khuyên bạn bắt đầu bằng cách chạy kịch bản ["tôi gặp sự cố khi gửi, nhận hoặc tìm thư email"](https://aka.ms/SaRA-OutlookSendReceive) từ công cụ [hỗ trợ của Microsoft và trợ lý phục hồi](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="6e490-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="6e490-104">Khi một thông báo bị kẹt trong hộp thư đi của bạn, các nguyên nhân có thể là:</span><span class="sxs-lookup"><span data-stu-id="6e490-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="6e490-105">Tệp đính kèm lớn.</span><span class="sxs-lookup"><span data-stu-id="6e490-105">Large attachments.</span></span>
- <span data-ttu-id="6e490-106">Tùy chọn **gửi ngay khi kết nối** không được kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="6e490-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="6e490-107">Để xóa tệp đính kèm lớn:</span><span class="sxs-lookup"><span data-stu-id="6e490-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="6e490-108">Trong Outlook, chọn **gửi/nhận** > **làm việc ngoại tuyến**.</span><span class="sxs-lookup"><span data-stu-id="6e490-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="6e490-109">Trong ngăn điều hướng, chọn **hộp**thư đi.</span><span class="sxs-lookup"><span data-stu-id="6e490-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="6e490-110">Từ đây, bạn có thể:</span><span class="sxs-lookup"><span data-stu-id="6e490-110">From here, you can:</span></span> 
    - <span data-ttu-id="6e490-111">Xoùa tin nhaén (chọn nó và sau đó chọn **Delete**).</span><span class="sxs-lookup"><span data-stu-id="6e490-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="6e490-112">Kéo thư vào thư mục bản thảo của bạn, bấm đúp để mở nó và xóa phần đính kèm, chọn nó rồi chọn **xóa**).</span><span class="sxs-lookup"><span data-stu-id="6e490-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="6e490-113">Nếu bạn nhận được lỗi cho biết Outlook đang cố truyền thư, đóng Outlook.</span><span class="sxs-lookup"><span data-stu-id="6e490-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="6e490-114">Có thể mất vài phút để thoát ra.</span><span class="sxs-lookup"><span data-stu-id="6e490-114">It may take a few moments to exit.</span></span> <span data-ttu-id="6e490-115">Nếu Outlook không đóng, nhấn Ctrl + Alt + Delete và chọn **khởi động trình quản lý tác vụ**.</span><span class="sxs-lookup"><span data-stu-id="6e490-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="6e490-116">Trong Task Manager, chọn tab **quá trình** , cuộn xuống Outlook. exe, và chọn **kết thúc tiến trình**.</span><span class="sxs-lookup"><span data-stu-id="6e490-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="6e490-117">Sau khi Outlook đóng, khởi động lại và lặp lại bước 2 và 3.</span><span class="sxs-lookup"><span data-stu-id="6e490-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="6e490-118">Sau khi bạn loại bỏ phần đính kèm, bấm **gửi/nhận** > **làm việc gián tuyến** để tiếp tục làm việc trực tuyến.</span><span class="sxs-lookup"><span data-stu-id="6e490-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="6e490-119">Thông báo cũng gặp khó khăn trong hộp thư đi khi bạn bấm vào **gửi**, nhưng bạn không được kết nối.</span><span class="sxs-lookup"><span data-stu-id="6e490-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="6e490-120">Nhấp vào **gửi/nhận** và xem nút **làm việc ngoại tuyến** .</span><span class="sxs-lookup"><span data-stu-id="6e490-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="6e490-121">Nếu màu xanh lam, bạn đã bị ngắt kết nối.</span><span class="sxs-lookup"><span data-stu-id="6e490-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="6e490-122">Chọn nó để kết nối (nút chuyển sang màu trắng) và nhấp vào **gửi tất cả**.</span><span class="sxs-lookup"><span data-stu-id="6e490-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="6e490-123">Để cho phép **gửi ngay lập tức khi kết nối**:</span><span class="sxs-lookup"><span data-stu-id="6e490-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="6e490-124">Chọn **tệp** > **tùy chọn** >  **nâng cao**.</span><span class="sxs-lookup"><span data-stu-id="6e490-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="6e490-125">Trong phần **gửi và nhận** , chọn **gửi ngay khi được kết nối**, sau đó chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="6e490-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="6e490-126">Để biết chi tiết đầy đủ xem:</span><span class="sxs-lookup"><span data-stu-id="6e490-126">For full details see:</span></span>
- [<span data-ttu-id="6e490-127">Video: gửi hoặc xóa một email bị kẹt</span><span class="sxs-lookup"><span data-stu-id="6e490-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="6e490-128">Email ở cặp hộp thư đi cho đến khi bạn tự bắt đầu hoạt động gửi/nhận trong Outlook</span><span class="sxs-lookup"><span data-stu-id="6e490-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
