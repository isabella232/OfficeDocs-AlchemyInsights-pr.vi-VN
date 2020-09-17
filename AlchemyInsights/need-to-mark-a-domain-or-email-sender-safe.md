---
title: Bạn cần đánh dấu tên miền hoặc người gửi email an toàn?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803267"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="527df-102">Bạn cần đánh dấu tên miền hoặc người gửi email an toàn?</span><span class="sxs-lookup"><span data-stu-id="527df-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="527df-103">Sử dụng **danh sách người gửi an toàn không được đề** xuất vì nó mở ra tổ chức của bạn để thư rác, phish và các cuộc tấn công giả mạo.</span><span class="sxs-lookup"><span data-stu-id="527df-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="527df-104">Tuy nhiên, nếu có một yêu cầu kinh doanh, chúng tôi **khuyên bạn nên** sử dụng các **[quy tắc dòng thư](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** cho điều này.</span><span class="sxs-lookup"><span data-stu-id="527df-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="527df-105">Hướng dẫn của chúng tôi đảm bảo xác thực người gửi (xác nhận tên miền gửi không được spoofed).</span><span class="sxs-lookup"><span data-stu-id="527df-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="527df-106">**Lưu ý**: chúng tôi không khuyên bạn nên quản lý tích cực false bằng cách sử dụng danh sách người gửi an toàn, vì ngoại lệ để lọc thư rác có thể mở tổ chức của bạn để bảo mật các cuộc tấn công.</span><span class="sxs-lookup"><span data-stu-id="527df-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="527df-107">Nếu người dùng của bạn nhận được thư không đúng được đánh dấu là thư rác hoặc email rác, vui lòng **[báo cáo các thư và tệp vào Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="527df-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="527df-108">Người gửi an toàn trong Outlook, danh sách người gửi được cho phép hoặc danh sách miền trong chính sách chống thư rác **sẽ bị tránh** vì người gửi bỏ qua tất cả các thư rác, spoof và bảo vệ bằng chữ và xác thực người gửi (SPF, DKIM, dMarc).</span><span class="sxs-lookup"><span data-stu-id="527df-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="527df-109">Phương pháp này chỉ được sử dụng tốt nhất để kiểm tra tạm thời.</span><span class="sxs-lookup"><span data-stu-id="527df-109">This method is best used for temporary testing only.</span></span>
