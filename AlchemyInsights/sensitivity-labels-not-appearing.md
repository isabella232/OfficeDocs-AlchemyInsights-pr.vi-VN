---
title: Không xuất hiện nhãn nhạy cảm
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801206"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="074a1-102">Không xuất hiện nhãn nhạy cảm</span><span class="sxs-lookup"><span data-stu-id="074a1-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="074a1-103">Nhãn nhạy cảm cho phép bạn phân loại và giúp bảo vệ nội dung nhạy cảm của bạn.</span><span class="sxs-lookup"><span data-stu-id="074a1-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="074a1-104">Chúng có thể được tạo trong Trung tâm tuân thủ Microsoft 365, Trung tâm bảo mật Microsoft 365, hoặc trung tâm tuân thủ & bảo mật của Microsoft 365 trong phân loại các nhãn nhạy cảm >.</span><span class="sxs-lookup"><span data-stu-id="074a1-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="074a1-105">Để tìm hiểu thêm về tính năng này, hãy xem mục [tổng quan về nhãn nhạy cảm](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="074a1-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="074a1-106">Nếu bạn cấu hình nhãn nhạy cảm nhưng không xuất hiện trong ứng dụng Microsoft 365, hãy kiểm tra các mục sau:</span><span class="sxs-lookup"><span data-stu-id="074a1-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="074a1-107">Xác nhận rằng nhãn nhạy cảm đã được [phát](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) hành cho người dùng và nhóm mà bạn muốn.</span><span class="sxs-lookup"><span data-stu-id="074a1-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="074a1-108">Xác nhận rằng người dùng đang sử dụng một ứng dụng hỗ trợ nhãn nhạy cảm-xem [nhãn nhạy cảm trong tài liệu của bạn](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="074a1-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="074a1-109">Nếu bạn đang [di chuyển nhãn bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), hãy lưu ý đến các cân nhắc được liệt kê [ở đây](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span><span class="sxs-lookup"><span data-stu-id="074a1-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="074a1-110">Bộ phận hỗ trợ ngăn mất dữ liệu: hiện tại, chỉ có thể sử dụng các nhãn duy trì như là một điều kiện trong các chính sách có quy định.</span><span class="sxs-lookup"><span data-stu-id="074a1-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="074a1-111">Hỗ trợ cho nhãn nhạy cảm trong chính sách không có sẵn nhưng vẫn chưa sẵn dùng nhưng chúng tôi đang làm việc trên đó.</span><span class="sxs-lookup"><span data-stu-id="074a1-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="074a1-112">Khi mã hóa được bật trên nhãn nhạy cảm, bạn có thể chọn:</span><span class="sxs-lookup"><span data-stu-id="074a1-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="074a1-113">Gán quyền ngay bây giờ</span><span class="sxs-lookup"><span data-stu-id="074a1-113">Assign permissions now</span></span>
    - <span data-ttu-id="074a1-114">Cho phép người dùng gán quyền</span><span class="sxs-lookup"><span data-stu-id="074a1-114">Let users assign permissions</span></span>


<span data-ttu-id="074a1-115">Để biết thêm thông tin về các vấn đề có thể xảy ra, hãy xem các [vấn đề đã biết với nhãn nhạy cảm](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="074a1-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>