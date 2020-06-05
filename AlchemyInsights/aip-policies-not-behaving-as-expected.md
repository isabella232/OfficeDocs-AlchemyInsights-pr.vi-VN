---
title: 'AIP: chính sách không phản bội như mong đợi'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 91308850c06485bdd11e81bd130770aefb247118
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580787"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="1fce1-102">AIP: chính sách không phản bội như mong đợi</span><span class="sxs-lookup"><span data-stu-id="1fce1-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="1fce1-103">Azure bảo vệ thông tin: chính sách không có như mong đợi, xem các hướng dẫn được khuyến nghị cho các vấn đề chính sách:</span><span class="sxs-lookup"><span data-stu-id="1fce1-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="1fce1-104">Nếu bạn đang gặp vấn đề với các dấu hiệu trực quan, vui lòng đánh giá [khi áp dụng](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)dấu hiệu hình ảnh.</span><span class="sxs-lookup"><span data-stu-id="1fce1-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="1fce1-105">Nếu bạn gặp sự cố với ghi nhãn tự động, vui lòng xem lại [cách cấu hình điều kiện để phân loại tự động và được đề xuất để bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) và [các loại thông tin nhạy cảm tìm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)kiếm.</span><span class="sxs-lookup"><span data-stu-id="1fce1-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="1fce1-106">Nếu bạn gặp vấn đề với Native/Pfile bảo vệ, hãy xem [tập tin cấu hình API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="1fce1-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="1fce1-107">Kiểm tra nếu bạn đang sử dụng chính sách scoped không được cấu hình đúng: [làm thế nào để cấu hình chính sách bảo vệ thông tin Azure cho người dùng cụ thể bằng cách sử dụng scoped chính sách](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="1fce1-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="1fce1-108">Nếu ghi nhãn tự động không hoạt động cho Outlook khi đính kèm một tài liệu có nhãn, xác minh rằng DRMEncryptProperty không được xác định như mô tả ở đây: [cài đặt đăng ký IRM cho bảo mật](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="1fce1-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="1fce1-109">Nếu bạn vẫn đang gặp sự cố, hãy thu thập Nhật ký khách hàng bảo vệ thông tin Azure và đính kèm Nhật ký xuất vé này.</span><span class="sxs-lookup"><span data-stu-id="1fce1-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="1fce1-110">Mở tài liệu Office hoặc tạo một email mới trong Outlook.</span><span class="sxs-lookup"><span data-stu-id="1fce1-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="1fce1-111">Nhấp vào **bảo vệ/**  >  **Trợ giúp độ nhạy và phản hồi**.</span><span class="sxs-lookup"><span data-stu-id="1fce1-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="1fce1-112">Nhấp vào **xuất Nhật ký**.</span><span class="sxs-lookup"><span data-stu-id="1fce1-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="1fce1-113">Lưu các bản ghi để lựa chọn vị trí của bạn, và đính kèm chúng vào yêu cầu dịch vụ này.</span><span class="sxs-lookup"><span data-stu-id="1fce1-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="1fce1-114">Tài nguyên bổ sung:</span><span class="sxs-lookup"><span data-stu-id="1fce1-114">Additional resources:</span></span>

- [<span data-ttu-id="1fce1-115">Làm thế nào để cấu hình nhãn cho dấu hiệu trực quan để bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="1fce1-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="1fce1-116">Đánh giá tài liệu về bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="1fce1-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="1fce1-117">Sử dụng nhãn nhạy cảm trong ứng dụng Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1fce1-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

