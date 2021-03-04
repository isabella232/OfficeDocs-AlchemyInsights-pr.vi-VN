---
title: Vấn đề với người dùng đơn lẻ
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430359"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="e4965-102">Vấn đề với người dùng đơn lẻ</span><span class="sxs-lookup"><span data-stu-id="e4965-102">Problem with single user</span></span>

- <span data-ttu-id="e4965-103">Người dùng có thể không được cung cấp bởi vì dịch vụ chưa có cơ hội đánh giá người dùng.</span><span class="sxs-lookup"><span data-stu-id="e4965-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="e4965-104">Xem lại hướng dẫn về cách cung cấp dài mất, cũng như thanh tiến độ trên trang cấu hình cung cấp.</span><span class="sxs-lookup"><span data-stu-id="e4965-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="e4965-105">Nếu trạng thái ổn định được xác định trong phần chi tiết bổ sung là trước ngày mà người dùng đã tạo/đã được Cập Nhật/đã xóa, điều đó có nghĩa là chúng tôi chưa đánh giá người dùng.</span><span class="sxs-lookup"><span data-stu-id="e4965-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="e4965-106">Trong trường hợp này, điều tốt nhất cần làm là chờ cho dịch vụ cung cấp để kết thúc.</span><span class="sxs-lookup"><span data-stu-id="e4965-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="e4965-107">Lưu ý rằng dịch vụ của chúng tôi chỉ nhận thức được những thay đổi đối với người dùng trong hệ thống nguồn (đám mây nhân sự).</span><span class="sxs-lookup"><span data-stu-id="e4965-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="e4965-108">Phải có thay đổi hợp lệ trong hệ thống nguồn cho Azure AD để phát hiện thay đổi và lưu nó thành Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e4965-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="e4965-109">Dịch vụ cung cấp sẽ đánh giá người dùng và xác định nó không nên được cung cấp:</span><span class="sxs-lookup"><span data-stu-id="e4965-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="e4965-110">Nếu bạn đã thiết lập bộ lọc dựa trên phạm vi thuộc tính, hãy đảm bảo rằng người dùng đáp ứng các tiêu chí mà bạn đã xác định.</span><span class="sxs-lookup"><span data-stu-id="e4965-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="e4965-111">Nếu người dùng đã tồn tại trong hệ thống đích và trạng thái của người dùng trong kết quả phù hợp với nguồn và đích, chúng tôi sẽ không thực hiện bất kỳ thao tác nào nữa.</span><span class="sxs-lookup"><span data-stu-id="e4965-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="e4965-112">Dịch vụ cung cấp đã tìm cách cung cấp cho người dùng và không thành công.</span><span class="sxs-lookup"><span data-stu-id="e4965-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="e4965-113">Đối với những tình huống này, hãy xem lại tab khắc phục sự cố và đề xuất của Nhật ký cung cấp:</span><span class="sxs-lookup"><span data-stu-id="e4965-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="e4965-114">Một thuộc tính bắt buộc trên người dùng có thể bị thiếu trong Active Directory tại chỗ hoặc Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e4965-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="e4965-115">Ví dụ, các quy tắc userPrincipalName hoặc sAMAccountName sẽ không tạo ra giá trị phù hợp.</span><span class="sxs-lookup"><span data-stu-id="e4965-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="e4965-116">Thuộc tính kết hợp (thường là employeeId) không giải quyết được một người dùng duy nhất trong Active Directory tại chỗ hoặc Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e4965-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="e4965-117">Ví dụ, có hai người dùng với cùng một employeeId trong quảng cáo và dịch vụ trả về một mã lỗi cho biết mục tiêu trùng lặp cho cùng một mục nhập nguồn.</span><span class="sxs-lookup"><span data-stu-id="e4965-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="e4965-118">Để xem lại Nhật ký dành cho người dùng và nhóm duy nhất, hãy xem [xem lại Nhật ký cung cấp cho vấn đề với một người dùng cụ thể](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span><span class="sxs-lookup"><span data-stu-id="e4965-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
