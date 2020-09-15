---
title: Dịch vụ 1048 5.7.750 không khả dụng. Máy khách bị chặn gửi từ các tên miền chưa đăng ký
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
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664264"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="178cb-103">máy khách 5.7.750 bị chặn không cho gửi từ tên miền chưa đăng ký</span><span class="sxs-lookup"><span data-stu-id="178cb-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="178cb-104">Lỗi xảy ra khi một lượng lớn các thư được gửi từ các tên miền không được cung cấp trong đối tượng thuê của bạn (Thêm tên miền được chấp nhận và xác thực).</span><span class="sxs-lookup"><span data-stu-id="178cb-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="178cb-105">Để tránh lỗi này, bạn có thể sử dụng đường kết nối dòng thư dựa trên chứng chỉ trong đó tên miền của chứng chỉ là miền được cung cấp, hoặc bạn có thể cung cấp tất cả các tên miền gửi.</span><span class="sxs-lookup"><span data-stu-id="178cb-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
