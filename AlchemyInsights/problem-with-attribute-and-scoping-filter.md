---
title: Sự cố với bộ lọc thuộc tính và phạm vi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482927"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="b38c7-102">Sự cố với bộ lọc thuộc tính và phạm vi</span><span class="sxs-lookup"><span data-stu-id="b38c7-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="b38c7-103">**Vấn đề với giá trị UPN xung đột**</span><span class="sxs-lookup"><span data-stu-id="b38c7-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="b38c7-104">Ngày làm việc cho người dùng quảng cáo cung cấp các ngày làm việc đến cấp phép người dùng quảng cáo hiển thị thông báo lỗi **Hybridsíp, Userprincipalnamenotunique**.</span><span class="sxs-lookup"><span data-stu-id="b38c7-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="b38c7-105">Thao tác không thành công vì giá trị UPN được cung cấp cho việc bổ sung/sửa đổi không phải là duy nhất toàn rừng.</span><span class="sxs-lookup"><span data-stu-id="b38c7-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="b38c7-106">Chi tiết lỗi: **CONSTRAINT_ATT_TYPE-userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="b38c7-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="b38c7-107">Giá trị **userPrincipalName** mà đường kết nối ngày làm việc đang cố gắng đặt khi tạo tài khoản người dùng quảng cáo đã tồn tại trong tên miền quảng cáo đích.</span><span class="sxs-lookup"><span data-stu-id="b38c7-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="b38c7-108">Điều này ngụ ý rằng một trong hai (1) người dùng đã tồn tại và ID kết hợp không thể kiểm tra được đối với người dùng hoặc (2) quy tắc thế hệ UPN tạo ra một giá trị xung đột.</span><span class="sxs-lookup"><span data-stu-id="b38c7-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="b38c7-109">Dưới đây là các bước giải quyết được đề xuất:</span><span class="sxs-lookup"><span data-stu-id="b38c7-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="b38c7-110">Nếu người dùng đã tồn tại và ID kết hợp sẽ không liên kết với tài khoản workday với tài khoản Active Directory, thì hãy kiểm tra xem liệu thuộc tính ID khớp (thường là **employeeID**) trong cả ngày làm việc và quảng cáo đều có kết quả khớp chính xác.</span><span class="sxs-lookup"><span data-stu-id="b38c7-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="b38c7-111">Nếu họ không có kết quả khớp, đó là một vấn đề dữ liệu cần được khắc phục.</span><span class="sxs-lookup"><span data-stu-id="b38c7-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="b38c7-112">Ví dụ, nếu EmployeeID trong ngày làm việc là 001052 và trong AD là 1052, thì công cụ cung cấp sẽ không liên kết hai tài khoản và sẽ cố gắng tạo một người dùng đã tồn tại.</span><span class="sxs-lookup"><span data-stu-id="b38c7-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="b38c7-113">Giải pháp trong trường hợp này là để thay đổi giá trị **EmployeeID** trong AD để đưa vào số không đứng đầu để làm cho nó 001052.</span><span class="sxs-lookup"><span data-stu-id="b38c7-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="b38c7-114">Nếu biểu thức tạo UPN không tạo ra một giá trị duy nhất, hãy cân nhắc việc sử dụng hàm de-trùng lặp **SelectUniqueValue** để tạo một giá trị duy nhất mỗi lần.</span><span class="sxs-lookup"><span data-stu-id="b38c7-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="b38c7-115">**Ngày làm việc cho người dùng quảng cáo không đặt giá trị thuộc tính Manager cho tài khoản người dùng quảng cáo**</span><span class="sxs-lookup"><span data-stu-id="b38c7-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="b38c7-116">Ngày làm việc đến người dùng quảng cáo sẽ không đặt giá trị thuộc tính **Manager** cho tài khoản người dùng quảng cáo.</span><span class="sxs-lookup"><span data-stu-id="b38c7-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="b38c7-117">Có hai tình huống có thể xảy ra khi hành vi này được nhìn thấy:</span><span class="sxs-lookup"><span data-stu-id="b38c7-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="b38c7-118">Trình quản lý trong ngày làm việc không thể được giải quyết cho tài khoản người dùng quảng cáo tương ứng vì người quản lý không nằm trong phạm vi.</span><span class="sxs-lookup"><span data-stu-id="b38c7-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="b38c7-119">Trong một kịch bản **nhiều tên miền quảng cáo** , trình quản lý trong ngày làm việc không có trong cùng tên miền với người dùng.</span><span class="sxs-lookup"><span data-stu-id="b38c7-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="b38c7-120">Hãy thử các bước sau để giải quyết vấn đề này:</span><span class="sxs-lookup"><span data-stu-id="b38c7-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="b38c7-121">Nếu bạn đã xác định bộ lọc có phạm vi, trước tiên, hãy kiểm tra xem người quản lý có được và điều đó thỏa mãn mệnh đề phạm vi hay không.</span><span class="sxs-lookup"><span data-stu-id="b38c7-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="b38c7-122">Nếu người quản lý không thỏa mãn bộ lọc có phạm vi, hãy thay đổi bộ lọc để người quản lý đó cũng có thể sử dụng thao tác cung cấp.</span><span class="sxs-lookup"><span data-stu-id="b38c7-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="b38c7-123">Nếu bạn có nhiều tên miền quảng cáo, thì đường kết nối có giới hạn đã biết không có khả năng giải quyết tham chiếu trình quản lý miền chéo.</span><span class="sxs-lookup"><span data-stu-id="b38c7-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="b38c7-124">Để biết thêm chi tiết về cách đặt cấu hình ngày làm việc cho tính năng cung cấp tự động, hãy xem [hướng dẫn: cấu hình ngày làm việc cho người dùng tự động cung](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)cấp.</span><span class="sxs-lookup"><span data-stu-id="b38c7-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













