---
title: Lỗi gửi thư điện tử bị chặn bởi SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29496775"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="baef1-102">Lỗi gửi thư điện tử: khách hàng lưu trữ bị chặn bằng cách sử dụng Spamhaus</span><span class="sxs-lookup"><span data-stu-id="baef1-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="baef1-p101">Địa chỉ IP gửi thư là một danh sách chặn thuộc sở hữu của [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Lý do bị chặn bởi Spamhaus bao gồm tài khoản bị xâm phạm, xâm nhập máy chia sẻ một địa chỉ IP công cộng, và các chính sách cung cấp dịch vụ Internet (ISP). Bản sửa lỗi có thể là:</span><span class="sxs-lookup"><span data-stu-id="baef1-p101">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies. Possible fixes are:</span></span>
  
- <span data-ttu-id="baef1-106">Chặn thư trong nước vào Office 365 mà bạn kiểm soát các máy chủ email mã nguồn, bạn cần phải xác định nguyên nhân gây ra và loại bỏ các khối từ trang web của Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="baef1-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="baef1-p102">Chặn thư trong nước vào Office 365 mà nguồn IP địa chỉ thuộc về người khác, chủ sở hữu của địa chỉ nhu cầu để loại bỏ khối từ trang web của Spamhaus. Nếu địa chỉ IP vào danh sách chặn chính sách (PBL), chủ sở hữu có thể gán một địa chỉ IP tĩnh khác nhau hoặc xóa địa chỉ khỏi PBL.</span><span class="sxs-lookup"><span data-stu-id="baef1-p102">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website. If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="baef1-p103">Chặn thư đi từ miền Office 365 của mình, bạn có thể nhận được lỗi này nếu thư được định tuyến thông qua một dịch vụ bên thứ 3. Bạn có thể sử dụng một công cụ tra cứu WHOIS để tìm chủ sở hữu địa chỉ IP bị chặn.</span><span class="sxs-lookup"><span data-stu-id="baef1-p103">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service. You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

