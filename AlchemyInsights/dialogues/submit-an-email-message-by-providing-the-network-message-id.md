---
title: Gửi thư email bằng cách cung cấp ID thông báo mạng
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695376"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="b2b70-102">Gửi thư email bằng cách cung cấp ID thông báo mạng</span><span class="sxs-lookup"><span data-stu-id="b2b70-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="b2b70-103">Trong các bản trình phát hành **mới** , hãy chọn **email** và **ID tin nhắn mạng**.</span><span class="sxs-lookup"><span data-stu-id="b2b70-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="b2b70-104">Hãy làm theo các bước sau đây để tìm thông điệp email trong Outlook:</span><span class="sxs-lookup"><span data-stu-id="b2b70-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="b2b70-105">Bấm đúp vào thông điệp email để mở.</span><span class="sxs-lookup"><span data-stu-id="b2b70-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="b2b70-106">Chọn   >  **thuộc tính** tệp.</span><span class="sxs-lookup"><span data-stu-id="b2b70-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="b2b70-107">Mở Notepad hoặc tài liệu Word trống, rồi sao chép và dán nội dung được tìm thấy trong hộp **tiêu đề Internet** vào tài liệu đang mở để có khả năng hiển thị tốt hơn.</span><span class="sxs-lookup"><span data-stu-id="b2b70-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="b2b70-108">Xác định vị trí trường **ID-MS-Exchange-tổ chức-thông tin thư** .</span><span class="sxs-lookup"><span data-stu-id="b2b70-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="b2b70-109">Giá trị sau **:** là ID bạn cần cho trình gửi của bạn.</span><span class="sxs-lookup"><span data-stu-id="b2b70-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="b2b70-110">Bên dưới **người nhận**, nếu email đã hạ cánh trong thư mục thư rác cho tất cả người nhận email này, hãy chọn **chọn tất cả**.</span><span class="sxs-lookup"><span data-stu-id="b2b70-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="b2b70-111">Nếu không, hãy chọn chỉ những người dùng đã báo cáo sự cố.</span><span class="sxs-lookup"><span data-stu-id="b2b70-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="b2b70-112">Bên dưới **lý do nộp hồ sơ**, nếu bạn chọn **nên đã bị chặn**, hãy chỉ rõ liệu thư nào có bị chặn là **thư rác**, **lừa đảo** qua mạng hay **phần mềm độc hại**, rồi chọn **gửi**.</span><span class="sxs-lookup"><span data-stu-id="b2b70-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="b2b70-113">Để tìm hiểu thêm, hãy xem [cách gửi thư rác bị nghi ngờ, phish, URL và tệp vào Microsoft để quét](https://go.microsoft.com/fwlink/?linkid=2101479).</span><span class="sxs-lookup"><span data-stu-id="b2b70-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
