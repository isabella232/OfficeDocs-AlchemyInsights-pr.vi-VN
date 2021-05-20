---
title: Tấn công Công cụ 2681 trong Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545748"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="15c82-102">Tấn công Phát hiện trong Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="15c82-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="15c82-103">Có phải bạn bỏ lỡ Tấn công Tấn công không?</span><span class="sxs-lookup"><span data-stu-id="15c82-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="15c82-104">Tính năng Tấn công **phải có Bộ bảo vệ Microsoft Office 365 Plan 2** hoặc Office 365 Enterprise **E5.**</span><span class="sxs-lookup"><span data-stu-id="15c82-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="15c82-105">Bảo vệ Tấn **công không** nằm trong Bộ bảo vệ Microsoft Office 365 Plan 1, Office 365 Enterprise E3 hoặc bất kỳ đăng ký Ứng dụng Microsoft 365 dành cho doanh nghiệp nào.</span><span class="sxs-lookup"><span data-stu-id="15c82-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="15c82-106">Tài khoản bạn sử dụng để khởi chạy các cuộc tấn công mô phỏng yêu cầu người quản trị toàn cầu hoặc người quản trị bảo mật phải có quyền của người quản trị bảo mật và xác thực đa yếu tố (MFA).</span><span class="sxs-lookup"><span data-stu-id="15c82-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="15c82-107">Để biết thêm thông tin về các yêu cầu đối với Tấn công đối với Tấn công, [hãy xem chủ đề này.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="15c82-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="15c82-108">Những điều quan trọng cần biết về **mô phỏng tấn công Brute Force Password:**</span><span class="sxs-lookup"><span data-stu-id="15c82-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="15c82-109">Nếu tài khoản đích đã bật MFA và mật khẩu đã được đoán đúng thì tài khoản sẽ không hiển thị là bị xâm phạm (hệ số xác thực thứ hai sẽ không hoàn tất).</span><span class="sxs-lookup"><span data-stu-id="15c82-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="15c82-110">Tệp mật khẩu không được lớn hơn 10 MB.</span><span class="sxs-lookup"><span data-stu-id="15c82-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="15c82-111">Sử dụng một mật khẩu cho mỗi dòng, và thêm một dòng trống (xuống dòng) sau mật khẩu cuối cùng trong danh sách.</span><span class="sxs-lookup"><span data-stu-id="15c82-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="15c82-112">Những điều quan trọng cần biết **về việc đính kèm mô** phỏng Lừa đảo qua hệ thống:</span><span class="sxs-lookup"><span data-stu-id="15c82-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="15c82-113">Theo chủ đích, bạn không thể cung cấp giá trị tùy chỉnh cho URL máy chủ đăng nhập Lừa đảo qua **mạng.**</span><span class="sxs-lookup"><span data-stu-id="15c82-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="15c82-114">Nếu người nhận [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) sử dụng phần bổ trợ Bật phần bổ trợ Thông báo Báo cáo để báo cáo thư là lừa đảo qua mạng, bạn có thể không nhận được cảnh báo về thư này (vì đây là một cuộc tấn công mô phỏng).</span><span class="sxs-lookup"><span data-stu-id="15c82-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="15c82-115">Báo cáo: Sau khi cuộc tấn công mô phỏng hoàn tất, bạn có thể bấm vào Chi **tiết Tấn** công để xem báo cáo.</span><span class="sxs-lookup"><span data-stu-id="15c82-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="15c82-116">Để biết hướng dẫn chi tiết và các tính năng mới trong Phát sinh Tấn công, xem [mục Tấn công Công cụ đối với Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="15c82-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
