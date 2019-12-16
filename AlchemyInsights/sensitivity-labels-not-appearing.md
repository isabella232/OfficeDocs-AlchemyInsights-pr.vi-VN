---
title: Nhãn độ nhạy không xuất hiện
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 67719380aea0481f96c03fa591542e8e5a6e6993
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048674"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="50f5f-102">Nhãn độ nhạy không xuất hiện</span><span class="sxs-lookup"><span data-stu-id="50f5f-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="50f5f-103">Nhãn nhạy cảm cho phép bạn phân loại và giúp bảo vệ nội dung nhạy cảm của mình.</span><span class="sxs-lookup"><span data-stu-id="50f5f-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="50f5f-104">Chúng có thể được tạo ra trong Trung tâm tuân thủ Microsoft 365, Trung tâm bảo mật Microsoft 365 hoặc văn phòng 365 bảo mật & Trung tâm tuân thủ phân loại > độ nhạy nhãn.</span><span class="sxs-lookup"><span data-stu-id="50f5f-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Office 365 Security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="50f5f-105">Để tìm hiểu thêm về tính năng này, hãy xem [tổng quan về các nhãn nhạy cảm](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="50f5f-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span></span>

<span data-ttu-id="50f5f-106">Nếu bạn đã định cấu hình nhãn nhạy cảm nhưng chúng không xuất hiện trong các ứng dụng Office, hãy kiểm tra sau:</span><span class="sxs-lookup"><span data-stu-id="50f5f-106">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="50f5f-107">Xác nhận rằng nhãn nhạy cảm đã được [xuất bản](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) cho người dùng và nhóm mà bạn muốn.</span><span class="sxs-lookup"><span data-stu-id="50f5f-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="50f5f-108">Xác nhận rằng người dùng đang sử dụng một ứng dụng hỗ trợ nhãn nhạy cảm-xem [nhãn nhạy cảm trong tài liệu của bạn](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="50f5f-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span></span>

- <span data-ttu-id="50f5f-109">Nếu bạn đang [di chuyển các nhãn bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), hãy lưu ý các cân nhắc được liệt kê [ở đây](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span><span class="sxs-lookup"><span data-stu-id="50f5f-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="50f5f-110">Hỗ trợ ngăn mất dữ liệu (DLP): hiện tại, chỉ các nhãn lưu giữ có thể được sử dụng làm điều kiện trong chính sách DLP.</span><span class="sxs-lookup"><span data-stu-id="50f5f-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="50f5f-111">Hỗ trợ cho các nhãn nhạy cảm trong chính sách DLP không có sẵn nhưng chúng tôi đang làm việc trên đó.</span><span class="sxs-lookup"><span data-stu-id="50f5f-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="50f5f-112">Khi mã hóa được bật trên nhãn nhạy cảm, bạn có thể chọn một trong hai cách:</span><span class="sxs-lookup"><span data-stu-id="50f5f-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="50f5f-113">Gán quyền ngay bây giờ</span><span class="sxs-lookup"><span data-stu-id="50f5f-113">Assign permissions now</span></span>
    - <span data-ttu-id="50f5f-114">Cho phép người dùng chỉ định quyền</span><span class="sxs-lookup"><span data-stu-id="50f5f-114">Let users assign permissions</span></span>


<span data-ttu-id="50f5f-115">Để biết thêm thông tin về vấn đề có thể xảy ra, xem [các vấn đề với độ nhạy nhãn](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="50f5f-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>