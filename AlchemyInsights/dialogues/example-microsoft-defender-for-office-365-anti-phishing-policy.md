---
title: Ví dụ về Microsoft Defender cho chính sách chống lừa đảo qua Office 365
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695636"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="55815-102">Ví dụ về Microsoft Defender cho chính sách chống lừa đảo qua Office 365</span><span class="sxs-lookup"><span data-stu-id="55815-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="55815-103">Các thiết đặt này cho phép một chính sách có tên là *Domain và CEO*.</span><span class="sxs-lookup"><span data-stu-id="55815-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="55815-104">Chính sách này cung cấp cho cả người dùng và bảo vệ tên miền khỏi mạo danh và sau đó áp dụng chính sách cho tất cả người dùng nhận được email bên trong tên miền.</span><span class="sxs-lookup"><span data-stu-id="55815-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="55815-105">Trước tiên, hãy thêm thông tin sau đây để tạo chính sách:</span><span class="sxs-lookup"><span data-stu-id="55815-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="55815-106">**Tên**: Domain và CEO **mô tả**: đảm bảo rằng giám đốc điều hành và tên miền của bạn đang không bị mạo danh.</span><span class="sxs-lookup"><span data-stu-id="55815-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="55815-107">Được **áp dụng cho**: chọn **tên miền của người nhận**.</span><span class="sxs-lookup"><span data-stu-id="55815-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="55815-108">Bên dưới **bất kỳ phần nào trong số này**, hãy chọn **chọn**, rồi chọn tên miền.</span><span class="sxs-lookup"><span data-stu-id="55815-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="55815-109">Chọn **+ Thêm**.</span><span class="sxs-lookup"><span data-stu-id="55815-109">Select **+ Add**.</span></span> <span data-ttu-id="55815-110">Chọn hộp kiểm bên cạnh tên miền trong danh sách (ví dụ, *contoso.com*), rồi chọn **Thêm**.</span><span class="sxs-lookup"><span data-stu-id="55815-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="55815-111">Chọn đã **xong**.</span><span class="sxs-lookup"><span data-stu-id="55815-111">Select **Done**.</span></span>
- <span data-ttu-id="55815-112">Sau khi chính sách được tạo ra, bạn có thể tinh chỉnh chính sách bằng cách sử dụng các tùy chọn sau đây:</span><span class="sxs-lookup"><span data-stu-id="55815-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="55815-113">**Thêm người dùng để bảo vệ:** Đối với ví dụ này, hãy thêm địa chỉ email của giám đốc điều hành, ở mức tối thiểu.</span><span class="sxs-lookup"><span data-stu-id="55815-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="55815-114">**Thêm tên miền để bảo vệ**: thêm tên miền tổ chức bao gồm Office của giám đốc điều hành.</span><span class="sxs-lookup"><span data-stu-id="55815-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="55815-115">**Chọn hành động**: **nếu email được gửi bởi người dùng mạo** danh, hãy chọn **chuyển hướng thư đến một địa chỉ email khác**, sau đó nhập địa chỉ email của người quản trị bảo mật (ví dụ, *securityadmin@contoso.com*).</span><span class="sxs-lookup"><span data-stu-id="55815-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="55815-116">**Nếu email được gửi bởi tên miền mạo** danh, hãy chọn cách **ly thư**.</span><span class="sxs-lookup"><span data-stu-id="55815-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="55815-117">**Thông minh trong hộp thư**: theo mặc định, tùy chọn này được chọn khi bạn tạo chính sách chống lừa đảo qua mạng mới.</span><span class="sxs-lookup"><span data-stu-id="55815-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="55815-118">Rời khỏi thiết đặt này để có kết quả **tốt nhất.**</span><span class="sxs-lookup"><span data-stu-id="55815-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="55815-119">**Thêm người gửi và tên miền đáng tin cậy:** Đối với ví dụ này, không xác định ghi đè.</span><span class="sxs-lookup"><span data-stu-id="55815-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="55815-120">Sau khi bạn đã xem lại các thiết đặt của mình, hãy chọn **tạo chính sách này** hoặc **lưu**, như phù hợp.</span><span class="sxs-lookup"><span data-stu-id="55815-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="55815-121">Để tìm hiểu thêm, hãy xem [chính sách chống lừa đảo trong Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span><span class="sxs-lookup"><span data-stu-id="55815-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
