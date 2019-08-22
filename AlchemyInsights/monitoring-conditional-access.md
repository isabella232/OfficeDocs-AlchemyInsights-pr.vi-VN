---
title: Giám sát truy cập có điều kiện
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538806"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="b74d4-102">Giám sát truy cập có điều kiện cho việc trao đổi</span><span class="sxs-lookup"><span data-stu-id="b74d4-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="b74d4-103">Nhắm mục tiêu với điều kiện truy cập người dùng sẽ nhận được một email thông báo nếu họ không đáp ứng yêu cầu truy cập tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="b74d4-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="b74d4-104">Để giải quyết, chúng tôi khuyên bạn nên một hoặc nhiều các giải pháp sau:</span><span class="sxs-lookup"><span data-stu-id="b74d4-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="b74d4-105">Nếu thiết bị là presumed để được đăng ký, tư vấn cho người sử dụng để đi đến các ứng dụng cổng thông tin công ty và xác minh rằng nó xuất hiện trong cổng công ty.</span><span class="sxs-lookup"><span data-stu-id="b74d4-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="b74d4-106">Nếu không, người dùng nên đăng ký các thiết bị.</span><span class="sxs-lookup"><span data-stu-id="b74d4-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="b74d4-107">Trong các cổng Azure vào **dành \> thiết bị tuân thủ**.</span><span class="sxs-lookup"><span data-stu-id="b74d4-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="b74d4-108">Trong **màn hình** nhấp vào **thiết bị tuân thủ**.</span><span class="sxs-lookup"><span data-stu-id="b74d4-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="b74d4-109">Xem báo cáo của bạn tuân thủ thiết bị để kiểm chứng rằng thiết bị của người dùng được đánh dấu như tuân thủ.</span><span class="sxs-lookup"><span data-stu-id="b74d4-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="b74d4-110">Trong các cổng Azure vào **dành \> thiết bị tuân thủ**.</span><span class="sxs-lookup"><span data-stu-id="b74d4-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="b74d4-111">Trong **quản lý**, bấm vào **chính sách**.</span><span class="sxs-lookup"><span data-stu-id="b74d4-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="b74d4-112">Trong danh sách các chính sách phù hợp, xác minh hồ sơ được gán cho thiết bị của người dùng.</span><span class="sxs-lookup"><span data-stu-id="b74d4-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="b74d4-113">Nếu hồ sơ không được phân công, sau đó dành sẽ không thể để xác nhận tình trạng tuân thủ của thiết bị.</span><span class="sxs-lookup"><span data-stu-id="b74d4-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="b74d4-114">Chỉnh sửa của người dùng truy cập có điều kiện chuyển nhượng.</span><span class="sxs-lookup"><span data-stu-id="b74d4-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="b74d4-115">Trong các cổng Azure vào **dành \> có điều kiện truy cập \> chính sách**</span><span class="sxs-lookup"><span data-stu-id="b74d4-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="b74d4-116">Chọn một chính sách từ danh sách</span><span class="sxs-lookup"><span data-stu-id="b74d4-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="b74d4-117">Nhấp vào **người dùng và nhóm**</span><span class="sxs-lookup"><span data-stu-id="b74d4-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="b74d4-118">Để nhắm mục tiêu một chính sách nhất định vào một ai đó, thêm chúng vào danh sách **bao gồm** .</span><span class="sxs-lookup"><span data-stu-id="b74d4-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="b74d4-119">Để đảm bảo rằng một người bỏ qua từ chính sách, thêm chúng vào danh sách **loại trừ** .</span><span class="sxs-lookup"><span data-stu-id="b74d4-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="b74d4-120">Đọc thêm: [làm thế nào để giám sát truy cập có điều kiện thiết bị](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="b74d4-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

