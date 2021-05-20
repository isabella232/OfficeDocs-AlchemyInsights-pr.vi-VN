---
title: Khắc phục sự cố về Bộ bảo vệ Microsoft Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545290"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="b1c96-102">Khắc phục sự cố về Bộ bảo vệ Microsoft Office 365</span><span class="sxs-lookup"><span data-stu-id="b1c96-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="b1c96-103">**Bạn có nhận thấy sự chậm trễ khi chuyển phát thư không?**</span><span class="sxs-lookup"><span data-stu-id="b1c96-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="b1c96-104">Sử dụng tùy [chọn Chuyển phát](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) động trong Bộ bảo vệ Microsoft để biết chính Office 365 Két sắt kèm.</span><span class="sxs-lookup"><span data-stu-id="b1c96-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="b1c96-105">Điều này sẽ giúp tránh tình trạng thư bị chậm trễ trong khi bảo vệ người nhận khỏi các tệp độc hại.</span><span class="sxs-lookup"><span data-stu-id="b1c96-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="b1c96-106">**Bạn có muốn báo cáo phủ nhận sai hay phủ nhận sai cho Microsoft không?**</span><span class="sxs-lookup"><span data-stu-id="b1c96-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="b1c96-107">Sử [dụng Trình khám phá Gửi.](https://protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="b1c96-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="b1c96-108">-\*\* Bạn có biết rằng bạn có thể bật bảo vệ liên kết Két sắt cho email nội bộ được gửi giữa những người nhận trong tổ chức của bạn không?\*\* Làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="b1c96-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="b1c96-109">Truy nhập và [https://protection.office.com](https://protection.office.com) đăng nhập bằng tài khoản người quản trị toàn cầu hoặc người quản trị bảo mật.</span><span class="sxs-lookup"><span data-stu-id="b1c96-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="b1c96-110">Trong ngăn điều hướng bên trái bên dưới Quản **lý mối đe dọa,** chọn **Chính sách** Két sắt liên \> **kết**.</span><span class="sxs-lookup"><span data-stu-id="b1c96-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="b1c96-111">Trong phần **Chính sách áp dụng cho toàn bộ tổ** chức, hãy chọn chính sách và bấm **Sửa**.</span><span class="sxs-lookup"><span data-stu-id="b1c96-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="b1c96-112">Trong Cài đặt **,** bật Áp **dụng liên kết an toàn cho các tin nhắn đã gửi trong tổ chức**.</span><span class="sxs-lookup"><span data-stu-id="b1c96-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
