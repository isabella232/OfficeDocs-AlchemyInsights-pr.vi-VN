---
title: Chính sách lưu giữ trong Trung tâm quản trị Exchange không hoạt động
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502629"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="4757e-102">Chính sách lưu giữ trong Trung tâm quản trị Exchange</span><span class="sxs-lookup"><span data-stu-id="4757e-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="4757e-103">**Vấn đề:** Chính sách mới được tạo hoặc Cập Nhật lưu giữ trong Trung tâm quản trị Exchange không áp dụng cho hộp thư hoặc các mục không được di chuyển vào hộp thư lưu trữ hoặc xoá.</span><span class="sxs-lookup"><span data-stu-id="4757e-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="4757e-104">**Nguyên nhân gốc:**</span><span class="sxs-lookup"><span data-stu-id="4757e-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="4757e-105">Điều này có thể do **hỗ trợ thư mục được quản lý** không xử lý hộp thư của người dùng.</span><span class="sxs-lookup"><span data-stu-id="4757e-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="4757e-106">Hỗ trợ thư mục được quản lý cố gắng xử lý mọi hộp thư trong tổ chức dựa trên ứng dụng web qua Internet của bạn một lần mỗi bảy ngày.</span><span class="sxs-lookup"><span data-stu-id="4757e-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="4757e-107">Nếu bạn thay đổi thẻ lưu giữ hoặc áp dụng chính sách lưu giữ khác cho hộp thư, bạn có thể đợi cho đến khi quản lý thư mục hỗ trợ quá trình hộp thư, hoặc bạn có thể chạy lệnh ghép ngắn Start-ManagedFolderAssistant khởi động hỗ trợ thư mục được quản lý để xử lý một hộp thư cụ thể.</span><span class="sxs-lookup"><span data-stu-id="4757e-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="4757e-108">Chạy lệnh ghép ngắn này rất hữu ích để kiểm tra hoặc khắc phục sự cố cài đặt chính sách lưu giữ hoặc thẻ lưu giữ.</span><span class="sxs-lookup"><span data-stu-id="4757e-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="4757e-109">Để biết thêm thông tin, hãy truy cập [chạy trình hỗ trợ thư mục được quản lý](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="4757e-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="4757e-110">**Giải pháp:** Chạy lệnh sau để khởi động hỗ trợ thư mục được quản lý cho một hộp thư cụ thể:</span><span class="sxs-lookup"><span data-stu-id="4757e-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="4757e-111">Điều này cũng có thể xảy ra nếu **RetentionHold** đã được **kích hoạt** trên hộp thư.</span><span class="sxs-lookup"><span data-stu-id="4757e-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="4757e-112">Nếu hộp thư đã được đặt trên một RetentionHold, chính sách lưu giữ trên hộp thư sẽ không được xử lý trong thời gian đó.</span><span class="sxs-lookup"><span data-stu-id="4757e-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="4757e-113">Để biết thêm Informaton trên thiết lập RetentionHold xem: giữ [hộp thư duy trì](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="4757e-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="4757e-114">**Giải pháp:**</span><span class="sxs-lookup"><span data-stu-id="4757e-114">**Solution:**</span></span>
    
  - <span data-ttu-id="4757e-115">Kiểm tra trạng thái của cài đặt RetentionHold trên hộp thư cụ thể trong [eXo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="4757e-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="4757e-116">Chạy lệnh sau để **vô hiệu hoá** RetentionHold trên một hộp thư cụ thể:</span><span class="sxs-lookup"><span data-stu-id="4757e-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="4757e-117">Bây giờ, chạy lại hỗ trợ thư mục được quản lý:</span><span class="sxs-lookup"><span data-stu-id="4757e-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="4757e-118">**Lưu ý:** Nếu hộp thư nhỏ hơn 10 MB, hỗ trợ thư mục được quản lý sẽ không tự động xử lý hộp thư.</span><span class="sxs-lookup"><span data-stu-id="4757e-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="4757e-119">Để biết thêm thông tin về chính sách lưu giữ trong Trung tâm quản trị Exchange, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="4757e-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="4757e-120">Chính sách lưu giữ và thẻ lưu giữ</span><span class="sxs-lookup"><span data-stu-id="4757e-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="4757e-121">Áp dụng chính sách lưu giữ cho hộp thư</span><span class="sxs-lookup"><span data-stu-id="4757e-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="4757e-122">Thêm hoặc xóa thẻ lưu giữ</span><span class="sxs-lookup"><span data-stu-id="4757e-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="4757e-123">Làm thế nào để xác định loại giữ được đặt trên hộp thư</span><span class="sxs-lookup"><span data-stu-id="4757e-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
