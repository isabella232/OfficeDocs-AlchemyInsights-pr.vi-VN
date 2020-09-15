---
title: 'AIP: chính sách không được điều hành như mong đợi'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663211"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="a818a-102">AIP: chính sách không được điều hành như mong đợi</span><span class="sxs-lookup"><span data-stu-id="a818a-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="a818a-103">Bảo vệ thông tin Azure: chính sách không được xử trị như mong đợi, hãy xem các hướng dẫn sau đây để được đề xuất cho các vấn đề chính sách khác nhau:</span><span class="sxs-lookup"><span data-stu-id="a818a-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="a818a-104">Nếu bạn đang gặp vấn đề với các dấu hiệu trực quan, vui lòng xem lại [khi áp dụng dấu hiệu trực quan](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="a818a-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="a818a-105">Nếu bạn đang gặp sự cố với việc ghi nhãn tự động, vui lòng xem lại [cách cấu hình các điều kiện cho việc phân loại thông tin và tự động cho Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) và [các kiểu thông tin nhạy cảm tìm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)kiếm.</span><span class="sxs-lookup"><span data-stu-id="a818a-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="a818a-106">Nếu bạn đang gặp vấn đề với việc bảo vệ bản địa/Pfile, vui lòng xem lại [cấu hình API tệp](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="a818a-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="a818a-107">Kiểm tra xem bạn đang sử dụng các chính sách phạm vi không được cấu hình đúng cách: [cách đặt cấu hình chính sách bảo vệ thông tin Azure cho những người dùng cụ thể bằng cách sử dụng các chính sách giới hạn](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="a818a-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="a818a-108">Nếu nhãn tự động không hoạt động cho Outlook khi đính kèm một tài liệu có nhãn, hãy xác minh rằng Drmencryptthuộc tính không được xác định như được mô tả ở đây: [thiết đặt đăng ký IRM cho bảo mật](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="a818a-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="a818a-109">Nếu bạn vẫn đang gặp phải vấn đề, vui lòng thu thập Nhật ký máy khách bảo vệ thông tin Azure và đính kèm các Nhật ký đã xuất ra vé này.</span><span class="sxs-lookup"><span data-stu-id="a818a-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="a818a-110">Mở tài liệu Office hoặc tạo email mới trong Outlook.</span><span class="sxs-lookup"><span data-stu-id="a818a-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="a818a-111">Bấm vào **bảo vệ/**  >  **Trợ giúp và phản hồi**nhạy cảm.</span><span class="sxs-lookup"><span data-stu-id="a818a-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="a818a-112">Bấm **xuất Nhật ký**.</span><span class="sxs-lookup"><span data-stu-id="a818a-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="a818a-113">Lưu Nhật ký vào lựa chọn vị trí của bạn và đính kèm chúng vào yêu cầu dịch vụ này.</span><span class="sxs-lookup"><span data-stu-id="a818a-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="a818a-114">Tài nguyên bổ sung:</span><span class="sxs-lookup"><span data-stu-id="a818a-114">Additional resources:</span></span>

- [<span data-ttu-id="a818a-115">Cách đặt cấu hình nhãn cho các dấu hiệu trực quan cho bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="a818a-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="a818a-116">Xem lại tài liệu bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="a818a-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="a818a-117">Sử dụng nhãn nhạy cảm trong ứng dụng Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a818a-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

