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
ms.openlocfilehash: b94fcc697bb7ac065cef57f3e3eb0b515c3094a0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35352875"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="eed2b-103">5.7.750 khách hàng chặn gửi từ chưa đăng ký tên miền</span><span class="sxs-lookup"><span data-stu-id="eed2b-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="eed2b-104">Lỗi xảy ra khi một lượng lớn các khối lượng của các thư được gửi từ các tên miền không được cung cấp trong Office 365 (Thêm vào như là miền được chấp nhận và xác nhận).</span><span class="sxs-lookup"><span data-stu-id="eed2b-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>

<span data-ttu-id="eed2b-105">Để tránh lỗi này, bạn có thể sử dụng một kết nối dòng dựa trên chứng chỉ thư, nơi các giấy chứng nhận tên miền là một miền được cung cấp, hoặc bạn có thể cung cấp tất cả các miền gửi.</span><span class="sxs-lookup"><span data-stu-id="eed2b-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
