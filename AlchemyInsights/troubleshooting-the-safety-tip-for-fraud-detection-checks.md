---
title: Khắc phục sự cố Mẹo an toàn cho phát hiện gian lận kiểm tra
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 7ce8bcc7caefebf51fc8d9622367fd16405deef1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533275"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="72c06-102">Khắc phục sự cố Mẹo an toàn cho phát hiện gian lận kiểm tra</span><span class="sxs-lookup"><span data-stu-id="72c06-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="72c06-103">Nếu bạn đang nhận được một Mẹo an toàn mà nói "người gửi không thành công của chúng tôi kiểm tra phát hiện gian lận và có thể không là những người họ xuất hiện để", sau đó người gửi không thành công để vượt qua kiểm tra xác thực DKIM hoặc SPF.</span><span class="sxs-lookup"><span data-stu-id="72c06-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="72c06-104">Các phương pháp tốt nhất để giải quyết điều này là dành cho người gửi cho phép bản thân mình.</span><span class="sxs-lookup"><span data-stu-id="72c06-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="72c06-105">Nếu người gửi gửi thay cho bạn, bạn cần phải cho phép chúng bằng cách thêm các địa chỉ IP của người gửi đến bản ghi SPF của bạn.</span><span class="sxs-lookup"><span data-stu-id="72c06-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="72c06-106">Xem [khắc phục sự cố Mẹo an toàn (nghi ngờ) màu đỏ cho phát hiện gian lận kiểm tra](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="72c06-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="72c06-107">Dưới đây là một số liên kết có thể giúp:</span><span class="sxs-lookup"><span data-stu-id="72c06-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="72c06-108">Cách Office 365 sử dụng khung chính sách người gửi (SPF) để ngăn chặn thư giả mạo</span><span class="sxs-lookup"><span data-stu-id="72c06-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="72c06-109">Thiết lập SPF trong Office 365 để giúp chặn thư giả mạo</span><span class="sxs-lookup"><span data-stu-id="72c06-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
