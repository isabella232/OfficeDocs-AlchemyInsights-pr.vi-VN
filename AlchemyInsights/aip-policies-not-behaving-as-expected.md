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
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506580"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="b5def-102">AIP: chính sách không phản bội như mong đợi</span><span class="sxs-lookup"><span data-stu-id="b5def-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="b5def-103">Azure bảo vệ thông tin: chính sách không có như mong đợi, xem các hướng dẫn được khuyến nghị cho các vấn đề chính sách:</span><span class="sxs-lookup"><span data-stu-id="b5def-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="b5def-104">Nếu bạn đang gặp vấn đề với các dấu hiệu trực quan, vui lòng đánh giá [khi áp dụng](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)dấu hiệu hình ảnh.</span><span class="sxs-lookup"><span data-stu-id="b5def-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="b5def-105">Nếu bạn gặp sự cố với ghi nhãn tự động, vui lòng xem lại [cách cấu hình điều kiện để phân loại tự động và được đề xuất để bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) và [các loại thông tin nhạy cảm tìm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)kiếm.</span><span class="sxs-lookup"><span data-stu-id="b5def-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="b5def-106">Nếu bạn gặp vấn đề với Native/Pfile bảo vệ, hãy xem [tập tin cấu hình API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="b5def-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="b5def-107">Kiểm tra nếu bạn đang sử dụng chính sách scoped không được cấu hình đúng: [làm thế nào để cấu hình chính sách bảo vệ thông tin Azure cho người dùng cụ thể bằng cách sử dụng scoped chính sách](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="b5def-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="b5def-108">Nếu ghi nhãn tự động không hoạt động cho Outlook khi đính kèm một tài liệu có nhãn, xác minh rằng DRMEncryptProperty không được xác định như mô tả ở đây: [cài đặt đăng ký IRM cho bảo mật](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="b5def-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="b5def-109">Nếu bạn vẫn đang gặp sự cố, hãy thu thập Nhật ký khách hàng bảo vệ thông tin Azure và đính kèm Nhật ký xuất vé này.</span><span class="sxs-lookup"><span data-stu-id="b5def-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="b5def-110">Mở tài liệu Office hoặc tạo một email mới trong Outlook.</span><span class="sxs-lookup"><span data-stu-id="b5def-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="b5def-111">Nhấp vào **bảo vệ/**  >  **Trợ giúp độ nhạy và phản hồi**.</span><span class="sxs-lookup"><span data-stu-id="b5def-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="b5def-112">Nhấp vào **xuất Nhật ký**.</span><span class="sxs-lookup"><span data-stu-id="b5def-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="b5def-113">Lưu các bản ghi để lựa chọn vị trí của bạn, và đính kèm chúng vào yêu cầu dịch vụ này.</span><span class="sxs-lookup"><span data-stu-id="b5def-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="b5def-114">Tài nguyên bổ sung:</span><span class="sxs-lookup"><span data-stu-id="b5def-114">Additional resources:</span></span>

- [<span data-ttu-id="b5def-115">Làm thế nào để cấu hình nhãn cho dấu hiệu trực quan để bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="b5def-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="b5def-116">Đánh giá tài liệu về bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="b5def-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="b5def-117">Sử dụng nhãn nhạy cảm trong ứng dụng Office</span><span class="sxs-lookup"><span data-stu-id="b5def-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

