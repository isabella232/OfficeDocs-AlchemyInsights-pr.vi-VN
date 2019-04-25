---
title: Lỗi gửi thư điện tử bị chặn bởi SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402281"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="611f1-102">Lỗi gửi thư điện tử: khách hàng lưu trữ bị chặn bằng cách sử dụng Spamhaus</span><span class="sxs-lookup"><span data-stu-id="611f1-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="611f1-103">Địa chỉ IP gửi thư là một danh sách chặn thuộc sở hữu của [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="611f1-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="611f1-104">Lý do bị chặn bởi Spamhaus bao gồm tài khoản bị xâm phạm, xâm nhập máy chia sẻ một địa chỉ IP công cộng, và các chính sách cung cấp dịch vụ Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="611f1-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="611f1-105">Bản sửa lỗi có thể là:</span><span class="sxs-lookup"><span data-stu-id="611f1-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="611f1-106">Chặn thư trong nước vào Office 365 mà bạn kiểm soát các máy chủ email mã nguồn, bạn cần phải xác định nguyên nhân gây ra và loại bỏ các khối từ trang web của Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="611f1-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="611f1-107">Chặn thư trong nước vào Office 365 mà nguồn IP địa chỉ thuộc về người khác, chủ sở hữu của địa chỉ nhu cầu để loại bỏ khối từ trang web của Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="611f1-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="611f1-108">Nếu địa chỉ IP vào danh sách chặn chính sách (PBL), chủ sở hữu có thể gán một địa chỉ IP tĩnh khác nhau hoặc xóa địa chỉ khỏi PBL.</span><span class="sxs-lookup"><span data-stu-id="611f1-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="611f1-109">Chặn thư đi từ miền Office 365 của mình, bạn có thể nhận được lỗi này nếu thư được định tuyến thông qua một dịch vụ bên thứ 3.</span><span class="sxs-lookup"><span data-stu-id="611f1-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="611f1-110">Bạn có thể sử dụng một công cụ tra cứu WHOIS để tìm chủ sở hữu địa chỉ IP bị chặn.</span><span class="sxs-lookup"><span data-stu-id="611f1-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

