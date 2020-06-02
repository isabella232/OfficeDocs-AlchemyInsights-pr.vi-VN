---
title: Khắc phục sự cố Office 365 nâng cao mối đe dọa bảo vệ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 7391b3c126d55213881f6b71cb6b5fc72bc68d0f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44512612"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="e786c-102">Khắc phục sự cố Office 365 nâng cao mối đe dọa bảo vệ</span><span class="sxs-lookup"><span data-stu-id="e786c-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="e786c-103">Bạn có nhận thấy sự chậm trễ trong việc gửi tin nhắn không?</span><span class="sxs-lookup"><span data-stu-id="e786c-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="e786c-104">Sử dụng tùy chọn [phân phối động](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) trong chính sách ATP an toàn đính kèm của bạn.</span><span class="sxs-lookup"><span data-stu-id="e786c-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="e786c-105">Điều này sẽ giúp tránh sự chậm trễ tin nhắn trong khi bảo vệ người nhận khỏi các tệp độc hại.</span><span class="sxs-lookup"><span data-stu-id="e786c-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="e786c-106">Bạn có muốn báo cáo sai tích cực hoặc sai phủ định cho Microsoft không?</span><span class="sxs-lookup"><span data-stu-id="e786c-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="e786c-107">Sử dụng [liên kết](https://www.microsoft.com/wdsi/filesubmission/) này để gửi tệp để phân tích.</span><span class="sxs-lookup"><span data-stu-id="e786c-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="e786c-108">Bạn có biết rằng bạn có thể bật bảo vệ liên kết an toàn cho email nội bộ được gửi giữa người nhận trong tổ chức của bạn?</span><span class="sxs-lookup"><span data-stu-id="e786c-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="e786c-109">Hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="e786c-109">Follow these steps:</span></span>

  1. <span data-ttu-id="e786c-110">Truy [https://protection.office.com](https://protection.office.com) cập và đăng nhập bằng tài khoản quản trị viên hoặc bảo mật toàn cầu.</span><span class="sxs-lookup"><span data-stu-id="e786c-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="e786c-111">Trong ngăn điều hướng bên trái trong **quản lý mối đe dọa**, hãy chọn **Policy** \> **liên kết an toàn**chính sách.</span><span class="sxs-lookup"><span data-stu-id="e786c-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="e786c-112">Trong **chính sách áp dụng cho toàn bộ phần tổ chức** , chọn chính sách và nhấp vào **chỉnh sửa**.</span><span class="sxs-lookup"><span data-stu-id="e786c-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="e786c-113">Trong **cài đặt**, **cho phép áp dụng liên kết an toàn cho thư được gửi trong tổ chức**.</span><span class="sxs-lookup"><span data-stu-id="e786c-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
