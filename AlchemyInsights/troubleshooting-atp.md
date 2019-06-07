---
title: Khắc phục sự cố Office 365 nâng cao mối đe dọa bảo vệ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: b4358fb55a1145833510c6063b520d822f2d1eaf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765559"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="558cf-102">Khắc phục sự cố Office 365 nâng cao mối đe dọa bảo vệ</span><span class="sxs-lookup"><span data-stu-id="558cf-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="558cf-103">Bạn có nhận thấy sự chậm trễ trong việc gửi thư?</span><span class="sxs-lookup"><span data-stu-id="558cf-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="558cf-104">Sử dụng các tùy chọn [Giao hàng năng động](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) trong chính sách ATP an toàn tập tin đính kèm của bạn.</span><span class="sxs-lookup"><span data-stu-id="558cf-104">Use the [Dynamic Delivery](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="558cf-105">Điều này sẽ giúp tránh sự chậm trễ thông báo trong khi bảo vệ người nhận từ các tập tin độc hại.</span><span class="sxs-lookup"><span data-stu-id="558cf-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="558cf-106">Bạn có muốn báo cáo sai tích cực hoặc tiêu cực sai để Microsoft?</span><span class="sxs-lookup"><span data-stu-id="558cf-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="558cf-107">Sử dụng [liên kết](https://www.microsoft.com/wdsi/filesubmission/) này để gửi các tập tin để phân tích.</span><span class="sxs-lookup"><span data-stu-id="558cf-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="558cf-108">Bạn có biết rằng bạn có thể cho phép bảo vệ an toàn các liên kết bên trong email được gửi giữa các người nhận trong tổ chức của bạn?</span><span class="sxs-lookup"><span data-stu-id="558cf-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="558cf-109">Hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="558cf-109">Follow these steps:</span></span>

  1. <span data-ttu-id="558cf-110">Đi đến [https://protection.office.com](https://protection.office.com) và đăng nhập bằng một người quản trị toàn cầu hoặc tài khoản quản trị an ninh.</span><span class="sxs-lookup"><span data-stu-id="558cf-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="558cf-111">Trong ngăn điều hướng bên trái quản lý **mối đe dọa**, chọn **chính sách** \> **Liên kết an toàn**.</span><span class="sxs-lookup"><span data-stu-id="558cf-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="558cf-112">Trong phần **chính sách áp dụng cho toàn bộ tổ chức** , chọn chính sách và nhấp vào **chỉnh sửa**.</span><span class="sxs-lookup"><span data-stu-id="558cf-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="558cf-113">Dưới **cài đặt**, cho phép **áp dụng an toàn các liên kết đến các tin nhắn được gửi trong tổ chức**.</span><span class="sxs-lookup"><span data-stu-id="558cf-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
