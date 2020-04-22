---
title: 1048 5.7.750 dịch vụ không khả dụng. Khách hàng bị chặn gửi từ tên miền chưa đăng ký
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 48b9c2de27f8d7f52215c3a3d547bdf746a3a4cd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676735"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="321d6-103">5.7.750 khách hàng bị chặn gửi từ tên miền chưa đăng ký</span><span class="sxs-lookup"><span data-stu-id="321d6-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="321d6-104">Lỗi xảy ra khi một số lượng lớn thư được gửi từ miền không cung cấp trong đối tượng thuê (được chấp nhận tên miền và xác thực).</span><span class="sxs-lookup"><span data-stu-id="321d6-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="321d6-105">Để tránh lỗi này, bạn có thể sử dụng kết nối dòng thư dựa trên chứng chỉ mà tên miền của chứng chỉ là một miền được cung cấp, hoặc bạn có thể điều khoản tất cả các miền gửi.</span><span class="sxs-lookup"><span data-stu-id="321d6-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
