---
title: Khắc phục sự cố Mẹo phát hiện gian lận
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658432"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="8979d-102">Khắc phục sự cố Mẹo phát hiện gian lận</span><span class="sxs-lookup"><span data-stu-id="8979d-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="8979d-103">Nếu bạn nhận được Mẹo an toàn cho biết "người gửi không thể kiểm tra phát hiện gian lận của chúng tôi và có thể không phải người mà họ xuất hiện là", thì người gửi không thể vượt qua hoặc kiểm tra xác thực SPF.</span><span class="sxs-lookup"><span data-stu-id="8979d-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="8979d-104">Phương pháp tốt nhất để giải quyết điều này là dành cho người gửi để ủy quyền cho mình.</span><span class="sxs-lookup"><span data-stu-id="8979d-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="8979d-105">Nếu người gửi đang gửi thay mặt cho bạn, bạn cần phải ủy quyền cho họ bằng cách thêm địa chỉ IP của người gửi vào bản ghi SPF của bạn.</span><span class="sxs-lookup"><span data-stu-id="8979d-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="8979d-106">Xem [khắc phục sự cố Mẹo an toàn màu đỏ (đáng ngờ) để kiểm tra việc phát hiện gian lận](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="8979d-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="8979d-107">Dưới đây là một số liên kết khác có thể trợ giúp:</span><span class="sxs-lookup"><span data-stu-id="8979d-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="8979d-108">Cách Microsoft sử dụng khung chính sách người gửi (SPF) để ngăn chặn thư giả mạo</span><span class="sxs-lookup"><span data-stu-id="8979d-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="8979d-109">Thiết lập SPF để giúp ngăn chặn giả mạo</span><span class="sxs-lookup"><span data-stu-id="8979d-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
