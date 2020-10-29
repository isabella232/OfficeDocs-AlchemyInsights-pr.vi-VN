---
title: trình mô phỏng tấn công 2681 trong Microsoft 365
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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801573"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="1c46f-102">Trình mô phỏng tấn công trong Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1c46f-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="1c46f-103">Bạn có thiếu mô phỏng tấn công không?</span><span class="sxs-lookup"><span data-stu-id="1c46f-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="1c46f-104">Trình mô phỏng tấn công yêu cầu **Microsoft Defender cho office 365 Plan 2 (ATP Plan 2)** hoặc **Office 365 Enterprise E5** .</span><span class="sxs-lookup"><span data-stu-id="1c46f-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5** .</span></span> <span data-ttu-id="1c46f-105">Trình mô phỏng tấn công **không** được bao gồm trong Microsoft Defender cho Office 365 Plan 1 (ATP Plan 1), Office 365 Enterprise E3, hoặc bất kỳ ứng dụng Microsoft 365 dành cho doanh nghiệp.</span><span class="sxs-lookup"><span data-stu-id="1c46f-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="1c46f-106">Tài khoản mà bạn sử dụng để khởi động các cuộc tấn công mô phỏng yêu cầu người quản trị toàn cầu hoặc các quyền của người quản trị bảo mật và xác thực đa yếu tố (MFA).</span><span class="sxs-lookup"><span data-stu-id="1c46f-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="1c46f-107">Để biết thêm thông tin về các yêu cầu về mô phỏng tấn công, hãy xem [chủ đề này](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="1c46f-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="1c46f-108">Những điều quan trọng cần biết về các mô phỏng tấn công **mật khẩu Brute Force** :</span><span class="sxs-lookup"><span data-stu-id="1c46f-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="1c46f-109">Nếu tài khoản đích đã bật MFA và mật khẩu đã được đoán đúng, tài khoản sẽ không hiển thị là bị xâm phạm (yếu tố xác thực thứ hai sẽ không hoàn thành).</span><span class="sxs-lookup"><span data-stu-id="1c46f-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="1c46f-110">Tệp mật khẩu không thể lớn hơn 10 MB.</span><span class="sxs-lookup"><span data-stu-id="1c46f-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="1c46f-111">Sử dụng một mật khẩu cho mỗi dòng, và bao gồm một đường trống (giao hàng trả về) sau khi mật khẩu cuối cùng trong danh sách.</span><span class="sxs-lookup"><span data-stu-id="1c46f-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="1c46f-112">Những điều quan trọng cần biết về các mô phỏng về **lừa đảo** qua mạng:</span><span class="sxs-lookup"><span data-stu-id="1c46f-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="1c46f-113">Theo thiết kế, bạn không thể cung cấp giá trị tùy chỉnh cho **URL của máy chủ đăng nhập giả mạo** .</span><span class="sxs-lookup"><span data-stu-id="1c46f-113">By design, you can't provide a custom value for **Phishing login server URL** .</span></span>

  - <span data-ttu-id="1c46f-114">Nếu người nhận sử dụng phần [bổ trợ bật thông báo báo cáo](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) để báo cáo thư là lừa đảo, bạn có thể không nhận được cảnh báo cho thư (vì đây là một cuộc tấn công mô phỏng).</span><span class="sxs-lookup"><span data-stu-id="1c46f-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="1c46f-115">Báo cáo: sau khi hoàn thành cuộc tấn công mô phỏng, bạn có thể bấm vào **chi tiết tấn công** để xem báo cáo.</span><span class="sxs-lookup"><span data-stu-id="1c46f-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="1c46f-116">Để biết hướng dẫn chi tiết và các tính năng mới trong tấn công Simulator, hãy xem [tấn công Simulator trong Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="1c46f-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
