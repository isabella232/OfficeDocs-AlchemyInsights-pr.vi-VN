---
title: Chính sách Duy trì trong Trung tâm Quản trị Exchange không hoạt động
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952250"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="fd001-102">Chính sách Duy trì trong Trung tâm Quản trị Exchange</span><span class="sxs-lookup"><span data-stu-id="fd001-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="fd001-103">Nếu bạn muốn chúng tôi chạy kiểm tra tự động cho các cài đặt được đề cập dưới đây, hãy chọn nút quay lại <-- ở đầu trang này, rồi nhập địa chỉ email của người dùng gặp sự cố với chính sách duy trì.</span><span class="sxs-lookup"><span data-stu-id="fd001-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="fd001-104">Nếu bạn gặp sự cố với chính sách duy trì trong Trung tâm Quản trị Exchange không áp dụng cho hộp thư hoặc các mục không di chuyển đến hộp thư lưu trữ, hãy kiểm tra các mục sau:</span><span class="sxs-lookup"><span data-stu-id="fd001-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="fd001-105">**Nguyên nhân gốc:**</span><span class="sxs-lookup"><span data-stu-id="fd001-105">**Root Causes:**</span></span>

- <span data-ttu-id="fd001-106">**Bộ trợ giúp Thư mục có** Quản lý chưa xử lý hộp thư của người dùng.</span><span class="sxs-lookup"><span data-stu-id="fd001-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="fd001-107">Trợ lý Thư mục có Quản lý cố gắng xử lý mỗi hộp thư trong tổ chức trên nền điện toán đám mây của bạn một lần bảy ngày một lần.</span><span class="sxs-lookup"><span data-stu-id="fd001-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="fd001-108">**Giải pháp:** Chạy Bộ trợ giúp Thư mục có Quản lý.</span><span class="sxs-lookup"><span data-stu-id="fd001-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="fd001-109">**RetentionHold** đã được **bật trên** hộp thư.</span><span class="sxs-lookup"><span data-stu-id="fd001-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="fd001-110">Nếu hộp thư đã được đặt trên Giữ lại, chính sách duy trì trên hộp thư sẽ không được xử lý trong thời gian đó.</span><span class="sxs-lookup"><span data-stu-id="fd001-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="fd001-111">**Giải pháp:** Kiểm tra trạng thái của cài đặt Giữ lại và cập nhật nếu cần.</span><span class="sxs-lookup"><span data-stu-id="fd001-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="fd001-112">Để biết chi tiết, hãy xem [Giữ lại Hộp thư](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="fd001-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="fd001-113">**Lưu ý:** Nếu một hộp thư nhỏ hơn 10 MB, Trợ lý Thư mục được Quản lý sẽ không tự động xử lý hộp thư đó.</span><span class="sxs-lookup"><span data-stu-id="fd001-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="fd001-114">Để biết thêm thông tin về chính sách duy trì trong Trung tâm Quản trị Exchange, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="fd001-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="fd001-115">Thẻ duy trì và chính sách duy trì</span><span class="sxs-lookup"><span data-stu-id="fd001-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="fd001-116">[Áp dụng chính sách duy trì cho hộp thư hoặc](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) Thêm hoặc loại bỏ thẻ duy [trì](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="fd001-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="fd001-117">Cách xác định loại giữ được đặt trên hộp thư</span><span class="sxs-lookup"><span data-stu-id="fd001-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
