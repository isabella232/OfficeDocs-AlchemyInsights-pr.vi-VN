---
title: Bạn cần đánh dấu một tên miền hoặc người gửi email an toàn?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281241"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="3989c-102">Bạn cần đánh dấu một tên miền hoặc người gửi email an toàn?</span><span class="sxs-lookup"><span data-stu-id="3989c-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="3989c-103">**Không nên sử dụng danh sách người gửi an toàn** vì nó mở ra tổ chức của bạn để thư rác, lừa, và giả mạo tấn công.</span><span class="sxs-lookup"><span data-stu-id="3989c-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="3989c-104">Tuy nhiên, nếu có yêu cầu kinh doanh, chúng tôi **khuyên bạn nên** sử dụng **[quy tắc luồng thư](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** cho điều này.</span><span class="sxs-lookup"><span data-stu-id="3989c-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="3989c-105">Hướng dẫn của chúng tôi đảm bảo xác thực người gửi (kiểm tra miền gửi không bị spoofed).</span><span class="sxs-lookup"><span data-stu-id="3989c-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="3989c-106">**Lưu ý**: chúng tôi không khuyên bạn nên quản lý sai tích cực bằng cách sử dụng danh sách người gửi an toàn, vì ngoại lệ để lọc thư rác có thể mở tổ chức của bạn để tấn công bảo mật.</span><span class="sxs-lookup"><span data-stu-id="3989c-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="3989c-107">Nếu (các) người dùng của bạn nhận được thư không đúng đánh dấu là spam hoặc email rác, vui lòng **[báo cáo tin nhắn và tệp cho Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="3989c-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="3989c-108">Người gửi an toàn trong Outlook, được phép gửi danh sách hoặc danh sách cho phép tên miền trong chính sách chống thư rác **nên tránh** bởi vì người gửi bỏ qua tất cả thư rác, giả mạo và bảo vệ phish và xác thực gửi (SPF, DKIM, dMarc).</span><span class="sxs-lookup"><span data-stu-id="3989c-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="3989c-109">Phương pháp này được sử dụng tốt nhất để kiểm tra tạm thời chỉ.</span><span class="sxs-lookup"><span data-stu-id="3989c-109">This method is best used for temporary testing only.</span></span>
