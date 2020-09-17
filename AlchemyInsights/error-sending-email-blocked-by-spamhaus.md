---
title: Lỗi khi gửi email bị SpamHaus chặn
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783825"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="a8b95-102">Lỗi gửi email: máy chủ khách đã bị chặn bằng SpamHaus</span><span class="sxs-lookup"><span data-stu-id="a8b95-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="a8b95-103">Địa chỉ IP đã gửi thư nằm trong danh sách chặn thuộc sở hữu của [SpamHaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="a8b95-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="a8b95-104">Các lý do bị truy nhập bởi SpamHaus bao gồm các tài khoản đã xâm phạm, các máy xâm phạm chia sẻ một địa chỉ IP công cộng và các chính sách nhà cung cấp dịch vụ Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="a8b95-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="a8b95-105">Các bản sửa lỗi có thể là:</span><span class="sxs-lookup"><span data-stu-id="a8b95-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="a8b95-106">Đối với các thư đã chặn trong đó bạn kiểm soát máy chủ email nguồn, bạn cần xác định nguyên nhân và loại bỏ khối từ trang web SpamHaus.</span><span class="sxs-lookup"><span data-stu-id="a8b95-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="a8b95-107">Đối với các thư đã chặn trong đó địa chỉ IP nguồn thuộc về người khác, chủ sở hữu địa chỉ cần loại bỏ khối từ trang web SpamHaus.</span><span class="sxs-lookup"><span data-stu-id="a8b95-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="a8b95-108">Nếu địa chỉ IP nằm trên danh sách khối chính sách (PBL), chủ sở hữu có thể gán địa chỉ IP tĩnh khác hoặc loại bỏ địa chỉ khỏi PBL.</span><span class="sxs-lookup"><span data-stu-id="a8b95-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="a8b95-109">Đối với các thư gửi đi từ tên miền của bạn được kết nối với Microsoft, bạn có thể nhận được lỗi này nếu các thư được định tuyến thông qua dịch vụ của bên thứ 3.</span><span class="sxs-lookup"><span data-stu-id="a8b95-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="a8b95-110">Bạn có thể sử dụng công cụ tra cứu WHOIS để tìm chủ sở hữu địa chỉ IP bị chặn.</span><span class="sxs-lookup"><span data-stu-id="a8b95-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
