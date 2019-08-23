---
title: Chính sách lưu giữ trong Exchange trung tâm quản trị không làm việc
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551365"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="90bb2-102">Chính sách lưu giữ trong Trung tâm quản trị Exchange</span><span class="sxs-lookup"><span data-stu-id="90bb2-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="90bb2-103">**Vấn đề:** Vừa được tạo ra hoặc Cập Nhật duy trì chính sách trong Trung tâm quản trị Exchange không áp dụng cho hộp thư hoặc mục không được chuyển đến hộp thư lưu trữ hoặc xóa bỏ.</span><span class="sxs-lookup"><span data-stu-id="90bb2-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="90bb2-104">**Nguyên nhân gốc rễ:**</span><span class="sxs-lookup"><span data-stu-id="90bb2-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="90bb2-105">Điều này có thể là do sự **Quản lý thư mục chương trình hỗ trợ** đã không xử lý hộp thư của người dùng.</span><span class="sxs-lookup"><span data-stu-id="90bb2-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="90bb2-106">Chương trình hỗ trợ thư mục quản lý cố xử lý từng thư trong tổ chức dựa trên đám mây của bạn một lần mỗi bảy ngày.</span><span class="sxs-lookup"><span data-stu-id="90bb2-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="90bb2-107">Nếu bạn thay đổi thẻ lưu giữ hoặc áp dụng một chính sách lưu giữ khác cho một hộp thư, bạn có thể đợi cho đến khi người quản lý thư mục hỗ trợ xử lý hộp thư, hoặc bạn có thể chạy lệnh ghép ngắn Start-ManagedFolderAssistant để bắt đầu các quản lý thư mục chương trình hỗ trợ xử lý cụ thể hộp thư.</span><span class="sxs-lookup"><span data-stu-id="90bb2-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="90bb2-108">Chạy lệnh ghép ngắn này là hữu ích để thử hay gỡ rối một chính sách lưu giữ hoặc cài đặt thẻ lưu giữ.</span><span class="sxs-lookup"><span data-stu-id="90bb2-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="90bb2-109">Để biết thêm chi tiết, truy cập vào [chạy chương trình hỗ trợ thư mục quản lý](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="90bb2-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="90bb2-110">**Giải pháp:** Chạy lệnh sau để bắt đầu các quản lý thư mục chương trình hỗ trợ cho một hộp thư cụ thể:</span><span class="sxs-lookup"><span data-stu-id="90bb2-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="90bb2-111">Này cũng có thể xảy ra nếu **RetentionHold** đã là **kích hoạt** trong hộp thư.</span><span class="sxs-lookup"><span data-stu-id="90bb2-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="90bb2-112">Nếu hộp thư đã được đặt trên một RetentionHold, chính sách lưu giữ trên hộp thư sẽ không được xử lý trong thời gian đó.</span><span class="sxs-lookup"><span data-stu-id="90bb2-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="90bb2-113">Cho thêm informaton vào xem cài đặt RetentionHold: [Hộp thư lưu trữ tổ chức](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="90bb2-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="90bb2-114">**Giải pháp:**</span><span class="sxs-lookup"><span data-stu-id="90bb2-114">**Solution:**</span></span>
    
  - <span data-ttu-id="90bb2-115">Kiểm tra tình trạng của các thiết lập RetentionHold trong hộp thư cụ thể trong [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="90bb2-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="90bb2-116">Hãy chạy lệnh sau để **vô hiệu hóa** RetentionHold trên một hộp thư cụ thể:</span><span class="sxs-lookup"><span data-stu-id="90bb2-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="90bb2-117">Bây giờ, chạy lại các thư mục được quản lý trợ lý:</span><span class="sxs-lookup"><span data-stu-id="90bb2-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="90bb2-118">**Lưu ý:** Nếu một hộp thư nhỏ hơn 10 MB, chương trình hỗ trợ thư mục quản lý sẽ không tự động xử lý hộp thư.</span><span class="sxs-lookup"><span data-stu-id="90bb2-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="90bb2-119">Để biết thêm chi tiết về chính sách lưu giữ trong Trung tâm quản trị Exchange, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="90bb2-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="90bb2-120">Thẻ lưu giữ và chính sách lưu giữ</span><span class="sxs-lookup"><span data-stu-id="90bb2-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="90bb2-121">Áp dụng một chính sách lưu giữ cho hộp thư</span><span class="sxs-lookup"><span data-stu-id="90bb2-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="90bb2-122">Thêm hoặc xoá thẻ lưu giữ</span><span class="sxs-lookup"><span data-stu-id="90bb2-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="90bb2-123">Làm thế nào để xác định loại của tổ chức được đặt trên một hộp thư</span><span class="sxs-lookup"><span data-stu-id="90bb2-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
