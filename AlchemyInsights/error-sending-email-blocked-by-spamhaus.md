---
title: Lỗi gửi email bị chặn bởi SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714280"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="8e5b6-102">Lỗi gửi email: máy chủ khách hàng bị chặn bằng cách sử dụng SpamHaus</span><span class="sxs-lookup"><span data-stu-id="8e5b6-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="8e5b6-103">Địa chỉ IP gửi thư là một danh sách chặn thuộc sở hữu của [SpamHaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="8e5b6-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="8e5b6-104">Lý do bị chặn bởi SpamHaus bao gồm các tài khoản xâm phạm, Máy chia sẻ địa chỉ IP công cộng và chính sách nhà cung cấp dịch vụ Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="8e5b6-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="8e5b6-105">Các bản sửa lỗi có thể là:</span><span class="sxs-lookup"><span data-stu-id="8e5b6-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="8e5b6-106">Đối với các thư bị chặn đến nơi bạn kiểm soát máy chủ email nguồn, bạn cần phải xác định nguyên nhân và loại bỏ khối từ trang web SpamHaus.</span><span class="sxs-lookup"><span data-stu-id="8e5b6-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="8e5b6-107">Đối với các thư đến bị chặn trong đó địa chỉ IP nguồn thuộc về người khác, chủ sở hữu địa chỉ cần loại bỏ khối từ trang web SpamHaus.</span><span class="sxs-lookup"><span data-stu-id="8e5b6-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="8e5b6-108">Nếu địa chỉ IP nằm trong danh sách chặn chính sách (PBL), chủ sở hữu có thể gán địa chỉ IP tĩnh khác hoặc xoá địa chỉ khỏi PBL.</span><span class="sxs-lookup"><span data-stu-id="8e5b6-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="8e5b6-109">Đối với các thư đi bị chặn từ miền của bạn kết nối với Microsoft, bạn có thể nhận được lỗi này nếu thư được định tuyến thông qua dịch vụ bên thứ ba.</span><span class="sxs-lookup"><span data-stu-id="8e5b6-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="8e5b6-110">Bạn có thể sử dụng công cụ tra cứu WHOIS để tìm chủ sở hữu địa chỉ IP bị chặn.</span><span class="sxs-lookup"><span data-stu-id="8e5b6-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
