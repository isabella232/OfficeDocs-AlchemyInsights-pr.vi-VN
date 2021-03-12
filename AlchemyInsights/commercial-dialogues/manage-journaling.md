---
title: Quản lý ghi nhật ký
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748670"
---
# <a name="manage-journaling"></a><span data-ttu-id="d84ce-102">Quản lý ghi nhật ký</span><span class="sxs-lookup"><span data-stu-id="d84ce-102">Manage journaling</span></span>

<span data-ttu-id="d84ce-103">Journaling có thể giúp tổ chức của bạn phản hồi các yêu cầu tuân thủ pháp lý, quy định và tổ chức bằng cách ghi liên lạc email đến và gửi đi.</span><span class="sxs-lookup"><span data-stu-id="d84ce-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="d84ce-104">Hãy nhớ:</span><span class="sxs-lookup"><span data-stu-id="d84ce-104">Keep in mind:</span></span>

* <span data-ttu-id="d84ce-105">Bạn cần có quyền quản lý [tổ chức](https://go.microsoft.com/fwlink/?linkid=2115259) và quản [lý bản ghi](https://go.microsoft.com/fwlink/?linkid=2115469) trước khi có thể quản lý journaling.</span><span class="sxs-lookup"><span data-stu-id="d84ce-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="d84ce-106">Bạn cần có một hộp thư Nhật ký và (tùy chọn) một hộp thư sẽ được đặt cấu hình thay thế.</span><span class="sxs-lookup"><span data-stu-id="d84ce-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="d84ce-107">Để tìm hiểu thêm, hãy xem mục [đặt cấu hình journaling trong Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span><span class="sxs-lookup"><span data-stu-id="d84ce-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="d84ce-108">Trong Exchange Online, có giới hạn số lượng quy tắc nhật ký mà bạn có thể tạo.</span><span class="sxs-lookup"><span data-stu-id="d84ce-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="d84ce-109">Để biết chi tiết, hãy xem [giới hạn về Nhật ký, giao thông và quy tắc hộp thư đến](https://go.microsoft.com/fwlink/?linkid=2115261).</span><span class="sxs-lookup"><span data-stu-id="d84ce-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="d84ce-110">Exchange Online không hỗ trợ việc cung cấp báo cáo Nhật ký vào một hộp thư Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="d84ce-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="d84ce-111">Bạn phải xác định địa chỉ email của hệ thống lưu trữ tại cơ sở hoặc dịch vụ lưu trữ bên thứ ba làm hộp thư ghi nhật ký.</span><span class="sxs-lookup"><span data-stu-id="d84ce-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
