---
title: Giám sát quyền truy nhập có điều kiện
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702925"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="1ab71-102">Giám sát quyền truy nhập có điều kiện cho Exchange</span><span class="sxs-lookup"><span data-stu-id="1ab71-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="1ab71-103">Người dùng được mục tiêu với quyền truy nhập có điều kiện sẽ nhận được email thông báo nếu họ không đáp ứng các yêu cầu truy nhập của tổ chức bạn.</span><span class="sxs-lookup"><span data-stu-id="1ab71-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="1ab71-104">Để giải quyết, chúng tôi khuyên bạn nên một hoặc nhiều giải pháp sau đây:</span><span class="sxs-lookup"><span data-stu-id="1ab71-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="1ab71-105">Nếu thiết bị được cho là đã đăng ký, hãy tư vấn cho người dùng để đi đến ứng dụng cổng thông tin công ty và xác minh rằng nó sẽ xuất hiện trong cổng thông tin công ty.</span><span class="sxs-lookup"><span data-stu-id="1ab71-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="1ab71-106">Nếu không, người dùng sẽ đăng ký thiết bị.</span><span class="sxs-lookup"><span data-stu-id="1ab71-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="1ab71-107">Trong cổng thông tin Azure, đi đến \*\* \> tuân thủ thiết bị InTune\*\*.</span><span class="sxs-lookup"><span data-stu-id="1ab71-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="1ab71-108">Bên dưới **giám sát** bấm **tuân thủ thiết bị**.</span><span class="sxs-lookup"><span data-stu-id="1ab71-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="1ab71-109">Xem báo cáo tuân thủ thiết bị của bạn để xác minh rằng thiết bị của người dùng được đánh dấu là phù hợp.</span><span class="sxs-lookup"><span data-stu-id="1ab71-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="1ab71-110">Trong cổng thông tin Azure, đi đến \*\* \> tuân thủ thiết bị InTune\*\*.</span><span class="sxs-lookup"><span data-stu-id="1ab71-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="1ab71-111">Bên dưới **quản lý**, bấm vào **chính sách**.</span><span class="sxs-lookup"><span data-stu-id="1ab71-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="1ab71-112">Trong danh sách các chính sách tuân thủ, hãy xác nhận hồ sơ được gán cho thiết bị của người dùng.</span><span class="sxs-lookup"><span data-stu-id="1ab71-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="1ab71-113">Nếu không có hồ sơ nào được phân công, thì InTune sẽ không thể xác nhận trạng thái tuân thủ của thiết bị.</span><span class="sxs-lookup"><span data-stu-id="1ab71-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="1ab71-114">Chỉnh sửa nhiệm vụ truy nhập có điều kiện của người dùng.</span><span class="sxs-lookup"><span data-stu-id="1ab71-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="1ab71-115">Trong cổng thông tin Azure, đi tới \*\* \> \> chính sách truy nhập InTune\*\* có điều kiện</span><span class="sxs-lookup"><span data-stu-id="1ab71-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="1ab71-116">Chọn một chính sách từ danh sách</span><span class="sxs-lookup"><span data-stu-id="1ab71-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="1ab71-117">Bấm vào **người dùng và nhóm**</span><span class="sxs-lookup"><span data-stu-id="1ab71-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="1ab71-118">Để nhắm đến một chính sách nhất định tại một ai đó, hãy thêm họ vào danh sách **bao gồm** .</span><span class="sxs-lookup"><span data-stu-id="1ab71-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="1ab71-119">Để đảm bảo rằng một người được bỏ qua khỏi chính sách, hãy thêm họ vào danh sách **loại trừ** .</span><span class="sxs-lookup"><span data-stu-id="1ab71-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="1ab71-120">Đọc thêm: [cách theo dõi các thiết bị truy nhập](https://docs.microsoft.com/intune/conditional-access-exchange-monitor) có điều kiện</span><span class="sxs-lookup"><span data-stu-id="1ab71-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

