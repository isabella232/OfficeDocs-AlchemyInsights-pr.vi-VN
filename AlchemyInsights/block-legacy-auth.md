---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685620"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="84568-102">Chặn xác thực kế thừa</span><span class="sxs-lookup"><span data-stu-id="84568-102">Blocking legacy authentication</span></span>

<span data-ttu-id="84568-103">Kế thừa xác thực là một thuật ngữ tham chiếu đến một yêu cầu xác thực được thực hiện bởi:</span><span class="sxs-lookup"><span data-stu-id="84568-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="84568-104">Máy khách Office cũ hơn không sử dụng xác thực hiện đại (ví dụ, ứng dụng khách Office 2010).</span><span class="sxs-lookup"><span data-stu-id="84568-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="84568-105">Bất kỳ máy khách nào sử dụng các giao thức thư kế thừa chẳng hạn như IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="84568-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="84568-106">Để biết thêm thông tin về cách chặn xác thực thừa kế và bật xác thực hiện đại, hãy tham khảo việc [chặn xác thực kế thừa](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="84568-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="84568-107">Mặc định bảo mật trong Azure Active Directory (Azure AD) giúp bảo vệ tổ chức của bạn dễ dàng hơn.</span><span class="sxs-lookup"><span data-stu-id="84568-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="84568-108">Mặc định bảo mật chứa thiết đặt bảo mật được cấu hình sẵn cho các cuộc tấn công phổ biến.</span><span class="sxs-lookup"><span data-stu-id="84568-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="84568-109">Để biết thêm thông tin về mặc định về bảo mật, hãy tham khảo mục [mặc định về bảo mật là gì?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="84568-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="84568-110">**Lưu ý**: nếu đối tượng thuê của bạn đã được tạo vào hoặc sau ngày 22 tháng 10, 2019, có thể bạn đang gặp phải hành vi mặc định bảo mật mới và đã có tính năng mặc định bảo mật được kích hoạt trong đối tượng thuê của bạn.</span><span class="sxs-lookup"><span data-stu-id="84568-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="84568-111">Trong một nỗ lực để bảo vệ tất cả người dùng của chúng tôi, mặc định bảo mật đang được triển khai cho tất cả các đối tượng thuê mới được tạo ra.</span><span class="sxs-lookup"><span data-stu-id="84568-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
