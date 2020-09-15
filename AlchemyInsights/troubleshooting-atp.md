---
title: Khắc phục sự cố bảo vệ mối đe dọa nâng cao của 365 Office
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
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658936"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="4294d-102">Khắc phục sự cố bảo vệ mối đe dọa nâng cao của 365 Office</span><span class="sxs-lookup"><span data-stu-id="4294d-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="4294d-103">Bạn có thấy sự chậm trễ trong việc chuyển phát thư không?</span><span class="sxs-lookup"><span data-stu-id="4294d-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="4294d-104">Sử dụng tùy chọn chuyển phát [động](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) trong chính sách tệp đính kèm an toàn trong ATP của bạn.</span><span class="sxs-lookup"><span data-stu-id="4294d-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="4294d-105">Điều này sẽ giúp tránh sự chậm trễ của thư khi bảo vệ người nhận khỏi các tệp độc hại.</span><span class="sxs-lookup"><span data-stu-id="4294d-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="4294d-106">Bạn có muốn báo cáo dương tính false hoặc âm sai đối với Microsoft không?</span><span class="sxs-lookup"><span data-stu-id="4294d-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="4294d-107">Sử dụng [liên kết](https://www.microsoft.com/wdsi/filesubmission/) này để gửi các tệp để phân tích.</span><span class="sxs-lookup"><span data-stu-id="4294d-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="4294d-108">Bạn có biết rằng bạn có thể cho phép bảo vệ liên kết an toàn cho email nội bộ được gửi giữa những người nhận trong tổ chức của mình không?</span><span class="sxs-lookup"><span data-stu-id="4294d-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="4294d-109">Làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="4294d-109">Follow these steps:</span></span>

  1. <span data-ttu-id="4294d-110">Đi đến [https://protection.office.com](https://protection.office.com) và đăng nhập bằng tài khoản người quản trị toàn cầu hoặc người quản trị bảo mật.</span><span class="sxs-lookup"><span data-stu-id="4294d-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="4294d-111">Trong ngăn dẫn hướng bên trái bên dưới **quản lý mối đe dọa**, chọn **Policy** \> **nối kết an toàn**chính sách.</span><span class="sxs-lookup"><span data-stu-id="4294d-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="4294d-112">Trong phần **chính sách áp dụng cho toàn bộ tổ chức** , hãy chọn chính sách và bấm **sửa**.</span><span class="sxs-lookup"><span data-stu-id="4294d-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="4294d-113">Bên dưới **thiết đặt**, **cho phép áp dụng nối kết an toàn cho thư được gửi trong tổ chức**.</span><span class="sxs-lookup"><span data-stu-id="4294d-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
