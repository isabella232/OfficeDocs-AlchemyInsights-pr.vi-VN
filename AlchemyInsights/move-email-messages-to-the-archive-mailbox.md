---
title: Di chuyển thư vào hộp thư lưu trữ
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747225"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="545e8-102">Di chuyển email sang hộp thư lưu trữ</span><span class="sxs-lookup"><span data-stu-id="545e8-102">Move email to the archive mailbox</span></span>
 
1. <span data-ttu-id="545e8-103">Xác nhận rằng một **lưu trữ hộp thư** đã được kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="545e8-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="545e8-104">Nếu không, sử dụng các bước trong [bài viết này](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) để kích hoạt hộp thư lưu trữ.</span><span class="sxs-lookup"><span data-stu-id="545e8-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="545e8-105">Lưu trữ tin nhắn tự động cho hộp thư lưu trữ, thẻ lưu giữ với hành động **di chuyển vào lưu trữ** phải được đặt để **áp dụng tự động cho từ khóa toàn bộ hộp thư (mặc định)**.</span><span class="sxs-lookup"><span data-stu-id="545e8-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="545e8-106">Sử dụng các bước dưới đây để tạo ra các từ khóa: [lưu trữ mặc định từ khóa](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span><span class="sxs-lookup"><span data-stu-id="545e8-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>
    
3. <span data-ttu-id="545e8-107">Tiếp theo, thêm **lưu trữ** thẻ chính sách lưu giữ của bạn.</span><span class="sxs-lookup"><span data-stu-id="545e8-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="545e8-108">Trong Trung tâm quản trị Exchange, chọn **Chính sách lưu giữ** > thêm **di chuyển vào lưu trữ thẻ** cho > chính sách **tiết kiệm**.</span><span class="sxs-lookup"><span data-stu-id="545e8-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span> 
    
4. <span data-ttu-id="545e8-109">Bây giờ [chỉ định chính sách lưu giữ](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) cho hộp thư người dùng cụ thể.</span><span class="sxs-lookup"><span data-stu-id="545e8-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="545e8-110">Chính sách tương tự sẽ được áp dụng cho cả **chính** và hộp thư **lưu trữ** .</span><span class="sxs-lookup"><span data-stu-id="545e8-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="545e8-111">Nó có thể là cần thiết để lực lượng quản lý thư mục chương trình hỗ trợ (MFA) chạy và áp dụng các thiết đặt mới cho hộp thư của người dùng.</span><span class="sxs-lookup"><span data-stu-id="545e8-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="545e8-112">Chạy lệnh sau đây trong khi [kết nối với EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) để bắt đầu các quản lý thư mục chương trình hỗ trợ cho một hộp thư cụ thể:</span><span class="sxs-lookup"><span data-stu-id="545e8-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="545e8-113">Để biết thêm chi tiết về thiết lập một chính sách lưu trữ, hãy xem [thiết lập một chính sách lưu trữ và xóa hộp thư](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="545e8-113">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

