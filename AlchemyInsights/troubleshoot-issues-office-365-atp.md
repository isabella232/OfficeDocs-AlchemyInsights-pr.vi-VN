---
title: Khắc phục sự cố với bảo vệ mối đe dọa nâng cao của Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758087"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="4f7c2-102">Khắc phục sự cố với Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="4f7c2-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="4f7c2-103">**Thông báo về sự chậm trễ khi gửi thư email**?</span><span class="sxs-lookup"><span data-stu-id="4f7c2-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="4f7c2-104">Hãy thử sử dụng tùy chọn chuyển phát động cho chính sách tệp đính kèm an toàn trong ATP của bạn.</span><span class="sxs-lookup"><span data-stu-id="4f7c2-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="4f7c2-105">Điều này sẽ tránh sự chậm trễ chuyển phát thư email trong khi bảo vệ người nhận từ các tệp độc hại.</span><span class="sxs-lookup"><span data-stu-id="4f7c2-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="4f7c2-106">**Bạn có muốn báo cáo dương tính false hoặc âm sai**không?</span><span class="sxs-lookup"><span data-stu-id="4f7c2-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="4f7c2-107">Sử dụng liên kết này để gửi tệp của bạn để phân tích: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="4f7c2-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="4f7c2-108">**Bạn có biết rằng bạn có thể bật bảo vệ các liên kết an toàn của ATP cho email được gửi giữa mọi người trong tổ chức của bạn**không?</span><span class="sxs-lookup"><span data-stu-id="4f7c2-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="4f7c2-109">Làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="4f7c2-109">Follow these steps:</span></span>
    1. <span data-ttu-id="4f7c2-110">Đi đến https://protection.office.com và đăng nhập.</span><span class="sxs-lookup"><span data-stu-id="4f7c2-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="4f7c2-111">Đi đến **Threat management**  >  **Policy**  >  **nối kết an toàn**chính sách quản lý mối đe dọa.</span><span class="sxs-lookup"><span data-stu-id="4f7c2-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="4f7c2-112">Bên dưới **chính sách áp dụng cho những người nhận cụ thể**, sửa (hoặc thêm) một chính sách.</span><span class="sxs-lookup"><span data-stu-id="4f7c2-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="4f7c2-113">Chọn **áp dụng nối kết an toàn cho thư được gửi trong tổ chức**.</span><span class="sxs-lookup"><span data-stu-id="4f7c2-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="4f7c2-114">Lưu chính sách của bạn và cho phép khoảng 30 phút để các thay đổi của bạn hoạt động như thế nào thông qua Trung tâm dữ liệu của bạn.</span><span class="sxs-lookup"><span data-stu-id="4f7c2-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="4f7c2-115">Để được trợ giúp thêm với ATP, hãy xem mục [bảo vệ mối đe dọa nâng cao của Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="4f7c2-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>