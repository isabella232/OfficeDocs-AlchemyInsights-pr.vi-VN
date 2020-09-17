---
title: Di chuyển thư email đến hộp thư lưu trữ
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799802"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="77593-102">Di chuyển email đến hộp thư lưu trữ</span><span class="sxs-lookup"><span data-stu-id="77593-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="77593-103">Nếu bạn muốn chúng tôi chạy kiểm tra tự động cho các thiết đặt được đề cập dưới đây, hãy chọn nút quay lại <--ở phía trên cùng của trang này, sau đó nhập địa chỉ email của người dùng có vấn đề chuyển email đến hộp thư lưu trữ của họ.</span><span class="sxs-lookup"><span data-stu-id="77593-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="77593-104">Xác nhận rằng **hộp thư lưu trữ** đã được bật chưa.</span><span class="sxs-lookup"><span data-stu-id="77593-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="77593-105">Nếu không, hãy làm theo các bước trong [bài viết này](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) để cho phép hộp thư lưu trữ.</span><span class="sxs-lookup"><span data-stu-id="77593-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="77593-106">Để tự động lưu trữ thư vào hộp thư lưu trữ, thẻ duy trì với hành động **di chuyển đến lưu trữ** phải được đặt **tự động áp dụng cho toàn bộ hộp thư (mặc định)**.</span><span class="sxs-lookup"><span data-stu-id="77593-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="77593-107">Hãy làm theo các bước sau đây để tạo thẻ: [thẻ mặc định lưu trữ](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="77593-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="77593-108">Tiếp theo, thêm thẻ **lưu trữ** vào chính sách duy trì của bạn.</span><span class="sxs-lookup"><span data-stu-id="77593-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="77593-109">Trong Trung tâm quản trị Exchange, hãy chọn **chính sách duy trì** > thêm **thẻ lưu vào thẻ lưu trữ** vào chính sách > **lưu**.</span><span class="sxs-lookup"><span data-stu-id="77593-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="77593-110">Bây giờ, [gán chính sách duy trì](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) cho hộp thư của người dùng cụ thể.</span><span class="sxs-lookup"><span data-stu-id="77593-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="77593-111">Chính sách này sẽ được áp dụng cho cả **chính** và hộp thư **lưu trữ** .</span><span class="sxs-lookup"><span data-stu-id="77593-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="77593-112">Có thể cần phải có hiệu lực trợ lý thư mục được quản lý (MFA) để chạy và áp dụng các thiết đặt mới cho hộp thư của người dùng.</span><span class="sxs-lookup"><span data-stu-id="77593-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="77593-113">Chạy lệnh sau đây khi được [kết nối với EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) để khởi động trợ lý thư mục được quản lý cho một hộp thư cụ thể:</span><span class="sxs-lookup"><span data-stu-id="77593-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="77593-114">Khởi động-ManagedFolderAssistant-Identity <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="77593-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="77593-115">Để biết thêm thông tin về việc thiết lập chính sách lưu trữ, hãy xem [thiết lập chính sách lưu trữ và xóa cho hộp thư](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="77593-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  