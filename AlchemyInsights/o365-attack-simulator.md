---
title: 2681 Attack Simulator trong Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713488"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="1462b-102">Attack Simulator trong Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1462b-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="1462b-103">Bạn có thiếu Attack Simulator?</span><span class="sxs-lookup"><span data-stu-id="1462b-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="1462b-104">Attack Simulator yêu cầu **office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** hoặc **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="1462b-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="1462b-105">Tấn công mô phỏng **không** được bao gồm trong Office 365 nâng cao mối đe dọa bảo vệ kế hoạch 1 (ATP kế hoạch 1), Office 365 Enterprise E3 hoặc bất kỳ Microsoft 365 ứng dụng cho đăng ký kinh doanh.</span><span class="sxs-lookup"><span data-stu-id="1462b-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="1462b-106">Tài khoản bạn sử dụng để khởi chạy các cuộc tấn công mô phỏng yêu cầu quản trị viên toàn cầu hoặc quyền quản trị viên bảo mật và xác thực đa yếu tố (MFA).</span><span class="sxs-lookup"><span data-stu-id="1462b-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="1462b-107">Để biết thêm thông tin về yêu cầu Attack Simulator, xem [chủ đề này](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="1462b-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="1462b-108">Những điều quan trọng cần biết về mô phỏng tấn công **Brute Force mật khẩu** :</span><span class="sxs-lookup"><span data-stu-id="1462b-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="1462b-109">Nếu tài khoản đích đã bật MFA và mật khẩu đã được đoán đúng, tài khoản sẽ không hiển thị là bị xâm phạm (yếu tố xác thực thứ hai sẽ không đầy đủ).</span><span class="sxs-lookup"><span data-stu-id="1462b-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="1462b-110">Tệp mật khẩu không thể lớn hơn 10 MB.</span><span class="sxs-lookup"><span data-stu-id="1462b-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="1462b-111">Sử dụng một mật khẩu cho mỗi dòng, và bao gồm một dòng trống (vận chuyển trở lại) sau khi mật khẩu cuối cùng trong danh sách.</span><span class="sxs-lookup"><span data-stu-id="1462b-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="1462b-112">Những điều quan trọng cần biết về mô phỏng gắn giả **mạo của Spear** :</span><span class="sxs-lookup"><span data-stu-id="1462b-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="1462b-113">Theo thiết kế, bạn không thể cung cấp giá trị tùy chỉnh cho **URL máy chủ đăng nhập lừa đảo**.</span><span class="sxs-lookup"><span data-stu-id="1462b-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="1462b-114">Nếu người nhận sử dụng trình [bổ trợ thông báo báo cáo](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) để báo cáo thư là lừa đảo, bạn có thể không nhận được thông báo cho thư này (vì đây là một cuộc tấn công mô phỏng).</span><span class="sxs-lookup"><span data-stu-id="1462b-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="1462b-115">Báo cáo: sau khi cuộc tấn công mô phỏng hoàn tất, bạn có thể nhấp **chi tiết tấn công** để xem báo cáo.</span><span class="sxs-lookup"><span data-stu-id="1462b-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="1462b-116">Để biết hướng dẫn chi tiết và các tính năng mới trong Attack Simulator, xem [Attack Simulator trong Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="1462b-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
