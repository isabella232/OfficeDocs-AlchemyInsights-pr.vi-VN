---
title: 1048 5.7.750 Dịch vụ không sẵn dùng. Máy khách bị chặn không cho gửi miền chưa được đăng ký
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 5879c5996a28e8e9e61c696c51e7c590d1245ba1
ms.sourcegitcommit: edb9be61ff8c4df2a600f70952f6fa731c2093a9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52774273"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="11a87-103">5.7.750 Máy khách bị chặn gửi từ miền chưa được đăng ký</span><span class="sxs-lookup"><span data-stu-id="11a87-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="11a87-104">Lỗi này xảy ra khi một lượng lớn thư được gửi từ các miền không được cung cấp trong đối tượng thuê của bạn (được thêm vào như tên miền được chấp nhận và đã xác thực).</span><span class="sxs-lookup"><span data-stu-id="11a87-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="11a87-105">Để tránh lỗi này, bạn có thể dùng bộ nối dòng thư dựa trên chứng chỉ mà tên miền của chứng chỉ là một tên miền được cung cấp, hoặc bạn có thể cung cấp tất cả các tên miền gửi.</span><span class="sxs-lookup"><span data-stu-id="11a87-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>

<span data-ttu-id="11a87-106">Để biết thêm thông tin, hãy xem mục Khắc phục sự cố chuyển phát email có mã lỗi [5.7.700 đến 5.7.750 trong Exchange Online.](https://go.microsoft.com/fwlink/?linkid=2164955)</span><span class="sxs-lookup"><span data-stu-id="11a87-106">For more information, see [Fix email delivery issues for error codes 5.7.700 through 5.7.750 in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span></span>