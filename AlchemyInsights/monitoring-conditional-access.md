---
title: Giám sát điều kiện truy cập
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713740"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="a47b1-102">Giám sát điều kiện truy cập cho Exchange</span><span class="sxs-lookup"><span data-stu-id="a47b1-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="a47b1-103">Người dùng nhắm mục tiêu với truy cập có điều kiện sẽ nhận được một email thông báo nếu họ không đáp ứng yêu cầu truy cập của tổ chức bạn.</span><span class="sxs-lookup"><span data-stu-id="a47b1-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="a47b1-104">Để giải quyết, chúng tôi khuyên bạn nên một hoặc nhiều giải pháp sau:</span><span class="sxs-lookup"><span data-stu-id="a47b1-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="a47b1-105">Nếu thiết bị được coi là được ghi danh, hãy tư vấn cho người dùng để truy cập ứng dụng cổng thông tin công ty và xác minh rằng nó xuất hiện trong cổng thông tin công ty.</span><span class="sxs-lookup"><span data-stu-id="a47b1-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="a47b1-106">Nếu không, người dùng nên đăng ký thiết bị.</span><span class="sxs-lookup"><span data-stu-id="a47b1-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="a47b1-107">Trong cổng Azure đi để **InTune \> thiết bị tuân thủ**.</span><span class="sxs-lookup"><span data-stu-id="a47b1-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="a47b1-108">Trong **màn hình** bấm vào **thiết bị tuân thủ**.</span><span class="sxs-lookup"><span data-stu-id="a47b1-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="a47b1-109">Xem báo cáo tuân thủ thiết bị của bạn để xác minh rằng thiết bị của người dùng được đánh dấu là tuân thủ.</span><span class="sxs-lookup"><span data-stu-id="a47b1-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="a47b1-110">Trong cổng Azure đi để **InTune \> thiết bị tuân thủ**.</span><span class="sxs-lookup"><span data-stu-id="a47b1-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="a47b1-111">Trong **quản lý**, bấm vào **chính sách**.</span><span class="sxs-lookup"><span data-stu-id="a47b1-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="a47b1-112">Trong danh sách các chính sách tuân thủ, hãy xác minh rằng hồ sơ được gán cho thiết bị của người dùng của bạn.</span><span class="sxs-lookup"><span data-stu-id="a47b1-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="a47b1-113">Nếu không có hồ sơ nào được chỉ định, thì InTune sẽ không thể xác nhận trạng thái tuân thủ của thiết bị.</span><span class="sxs-lookup"><span data-stu-id="a47b1-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="a47b1-114">Chỉnh sửa gán quyền truy cập có điều kiện của người dùng.</span><span class="sxs-lookup"><span data-stu-id="a47b1-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="a47b1-115">Trong cổng Azure đi để **InTune \> điều kiện truy \> cập chính sách**</span><span class="sxs-lookup"><span data-stu-id="a47b1-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="a47b1-116">Chọn một chính sách từ danh sách</span><span class="sxs-lookup"><span data-stu-id="a47b1-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="a47b1-117">Nhấp vào **người dùng và nhóm**</span><span class="sxs-lookup"><span data-stu-id="a47b1-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="a47b1-118">Để nhắm mục tiêu một chính sách nhất định tại một người nào đó, hãy thêm chúng vào danh sách **bao gồm** .</span><span class="sxs-lookup"><span data-stu-id="a47b1-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="a47b1-119">Để đảm bảo rằng một người bị bỏ qua khỏi chính sách, hãy thêm họ vào danh sách **loại trừ** .</span><span class="sxs-lookup"><span data-stu-id="a47b1-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="a47b1-120">Đọc thêm: [cách giám sát các thiết bị truy cập có điều kiện](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="a47b1-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

