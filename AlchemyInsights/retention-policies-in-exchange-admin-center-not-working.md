---
title: Chính sách duy trì trong Trung tâm quản trị Exchange không hoạt động
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740532"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="e480f-102">Chính sách duy trì trong Trung tâm quản trị Exchange</span><span class="sxs-lookup"><span data-stu-id="e480f-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="e480f-103">Nếu bạn muốn chúng tôi chạy kiểm tra tự động cho các thiết đặt được đề cập dưới đây, hãy chọn nút quay lại <--ở phía trên cùng của trang này, sau đó nhập địa chỉ email của người dùng có vấn đề với chính sách duy trì.</span><span class="sxs-lookup"><span data-stu-id="e480f-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="e480f-104">**Vấn đề:** Các chính sách duy trì mới được tạo hoặc Cập Nhật trong Trung tâm quản trị Exchange không áp dụng cho các hộp thư hoặc mục sẽ không được di chuyển đến hộp thư lưu trữ hoặc bị xóa.</span><span class="sxs-lookup"><span data-stu-id="e480f-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="e480f-105">**Nguyên nhân gốc:**</span><span class="sxs-lookup"><span data-stu-id="e480f-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="e480f-106">Điều này có thể do **trợ lý thư mục được quản lý** không xử lý hộp thư của người dùng.</span><span class="sxs-lookup"><span data-stu-id="e480f-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="e480f-107">Trợ lý thư mục được quản lý cố gắng xử lý tất cả các hộp thư trong tổ chức dựa trên nền tảng điện toán đám mây của bạn một lần mỗi bảy ngày.</span><span class="sxs-lookup"><span data-stu-id="e480f-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="e480f-108">Nếu bạn thay đổi thẻ duy trì hoặc áp dụng chính sách duy trì khác vào hộp thư, bạn có thể đợi cho đến khi thư mục được quản lý hỗ trợ quy trình hộp thư hoặc bạn có thể chạy lệnh ghép ngắn Start-ManagedFolderAssistant để bắt đầu bộ trợ giúp thư mục được quản lý để xử lý một hộp thư cụ thể.</span><span class="sxs-lookup"><span data-stu-id="e480f-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="e480f-109">Chạy lệnh ghép ngắn này rất hữu ích cho việc thử nghiệm hoặc khắc phục sự cố các thiết đặt thẻ duy trì hoặc chính sách duy trì.</span><span class="sxs-lookup"><span data-stu-id="e480f-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="e480f-110">Để biết thêm thông tin, hãy truy cập [chạy trình trợ giúp thư mục được quản lý](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="e480f-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="e480f-111">**Giải pháp:** Chạy lệnh sau đây để bắt đầu trợ lý thư mục được quản lý cho một hộp thư cụ thể:</span><span class="sxs-lookup"><span data-stu-id="e480f-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="e480f-112">Điều này cũng có thể xảy ra nếu **RetentionHold** đã được **kích hoạt** trên hộp thư.</span><span class="sxs-lookup"><span data-stu-id="e480f-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="e480f-113">Nếu hộp thư đã được đặt trên một RetentionHold, chính sách duy trì trên hộp thư sẽ không được xử lý trong thời gian đó.</span><span class="sxs-lookup"><span data-stu-id="e480f-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="e480f-114">Để biết thêm thông tin chi tiết về cài đặt RetentionHold, hãy xem: [giữ duy trì hộp thư](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="e480f-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="e480f-115">**Nghiệm**</span><span class="sxs-lookup"><span data-stu-id="e480f-115">**Solution:**</span></span>
    
  - <span data-ttu-id="e480f-116">Kiểm tra trạng thái của thiết đặt RetentionHold trên hộp thư cụ thể trong [eXo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="e480f-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="e480f-117">Chạy lệnh sau đây để **vô hiệu hóa** RetentionHold trên một hộp thư cụ thể:</span><span class="sxs-lookup"><span data-stu-id="e480f-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="e480f-118">Bây giờ, hãy chạy lại trợ lý thư mục được quản lý:</span><span class="sxs-lookup"><span data-stu-id="e480f-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="e480f-119">**Lưu ý:** Nếu một hộp thư nhỏ hơn 10 MB, trợ lý thư mục được quản lý sẽ không tự động xử lý hộp thư.</span><span class="sxs-lookup"><span data-stu-id="e480f-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="e480f-120">Để biết thêm thông tin về chính sách duy trì trong Trung tâm quản trị Exchange, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="e480f-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="e480f-121">Thẻ duy trì và chính sách duy trì</span><span class="sxs-lookup"><span data-stu-id="e480f-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="e480f-122">Áp dụng chính sách duy trì cho hộp thư</span><span class="sxs-lookup"><span data-stu-id="e480f-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="e480f-123">Thêm hoặc loại bỏ thẻ duy trì</span><span class="sxs-lookup"><span data-stu-id="e480f-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="e480f-124">Cách xác định loại giữ được đặt trên một hộp thư</span><span class="sxs-lookup"><span data-stu-id="e480f-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
