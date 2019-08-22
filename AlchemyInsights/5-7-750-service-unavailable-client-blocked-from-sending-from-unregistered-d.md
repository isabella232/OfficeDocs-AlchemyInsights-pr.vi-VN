---
title: 1048 5.7.750 dịch vụ không sẵn dùng. Khách hàng bị chặn gửi từ các tên miền chưa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 7126b4de7f7d8861afdb22af2540d6910c1d014f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494477"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="e9f63-103">5.7.750 khách hàng chặn gửi từ chưa đăng ký tên miền</span><span class="sxs-lookup"><span data-stu-id="e9f63-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="e9f63-104">Lỗi xảy ra khi một lượng lớn các khối lượng của các thư được gửi từ các tên miền không được cung cấp trong Office 365 (Thêm vào như là miền được chấp nhận và xác nhận).</span><span class="sxs-lookup"><span data-stu-id="e9f63-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>

<span data-ttu-id="e9f63-105">Để tránh lỗi này, bạn có thể sử dụng một kết nối dòng dựa trên chứng chỉ thư, nơi các giấy chứng nhận tên miền là một miền được cung cấp, hoặc bạn có thể cung cấp tất cả các miền gửi.</span><span class="sxs-lookup"><span data-stu-id="e9f63-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
