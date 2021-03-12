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
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708696"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="4d888-102">Giám sát quyền truy nhập có điều kiện cho Exchange</span><span class="sxs-lookup"><span data-stu-id="4d888-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="4d888-103">Người dùng được mục tiêu với quyền truy nhập có điều kiện sẽ nhận được email thông báo nếu họ không đáp ứng các yêu cầu truy nhập của tổ chức bạn.</span><span class="sxs-lookup"><span data-stu-id="4d888-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="4d888-104">Để giải quyết, chúng tôi khuyên bạn nên một hoặc nhiều giải pháp sau đây:</span><span class="sxs-lookup"><span data-stu-id="4d888-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="4d888-105">Nếu thiết bị được cho là đã đăng ký, hãy tư vấn cho người dùng để đi đến ứng dụng cổng thông tin công ty và xác minh rằng nó sẽ xuất hiện trong cổng thông tin công ty.</span><span class="sxs-lookup"><span data-stu-id="4d888-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="4d888-106">Nếu không, người dùng sẽ đăng ký thiết bị.</span><span class="sxs-lookup"><span data-stu-id="4d888-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="4d888-107">Trong cổng thông tin Azure, đi tới InTune > tuân thủ thiết bị.</span><span class="sxs-lookup"><span data-stu-id="4d888-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="4d888-108">Bên dưới giám sát bấm tuân thủ thiết bị.</span><span class="sxs-lookup"><span data-stu-id="4d888-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="4d888-109">Xem báo cáo tuân thủ thiết bị của bạn để xác minh rằng thiết bị của người dùng được đánh dấu là phù hợp.</span><span class="sxs-lookup"><span data-stu-id="4d888-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="4d888-110">Trong cổng thông tin Azure, đi tới InTune > tuân thủ thiết bị.</span><span class="sxs-lookup"><span data-stu-id="4d888-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="4d888-111">Bên dưới quản lý, bấm vào chính sách.</span><span class="sxs-lookup"><span data-stu-id="4d888-111">Under Manage, click Policies.</span></span> <span data-ttu-id="4d888-112">Trong danh sách các chính sách tuân thủ, hãy xác nhận hồ sơ được gán cho thiết bị của người dùng.</span><span class="sxs-lookup"><span data-stu-id="4d888-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="4d888-113">Nếu không có hồ sơ nào được phân công, thì InTune sẽ không thể xác nhận trạng thái tuân thủ của thiết bị.</span><span class="sxs-lookup"><span data-stu-id="4d888-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="4d888-114">Chỉnh sửa nhiệm vụ truy nhập có điều kiện của người dùng.</span><span class="sxs-lookup"><span data-stu-id="4d888-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="4d888-115">Trong cổng thông tin Azure, đi tới  >    >  **chính sách** truy nhập InTune có điều kiện.</span><span class="sxs-lookup"><span data-stu-id="4d888-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="4d888-116">Chọn một chính sách từ danh sách.</span><span class="sxs-lookup"><span data-stu-id="4d888-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="4d888-117">Bấm vào người dùng và nhóm.</span><span class="sxs-lookup"><span data-stu-id="4d888-117">Click Users and groups.</span></span>
4. <span data-ttu-id="4d888-118">Để nhắm đến một chính sách nhất định tại một ai đó, hãy thêm họ vào danh sách bao gồm.</span><span class="sxs-lookup"><span data-stu-id="4d888-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="4d888-119">Để đảm bảo rằng một người được bỏ qua khỏi chính sách, hãy thêm họ vào danh sách loại trừ.</span><span class="sxs-lookup"><span data-stu-id="4d888-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="4d888-120">Liên kết hữu ích:</span><span class="sxs-lookup"><span data-stu-id="4d888-120">Helpful links:</span></span>

[<span data-ttu-id="4d888-121">Tổng quan về tuân thủ thiết bị</span><span class="sxs-lookup"><span data-stu-id="4d888-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="4d888-122">Khắc phục sự cố</span><span class="sxs-lookup"><span data-stu-id="4d888-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="4d888-123">Chính sách khắc phục sự cố</span><span class="sxs-lookup"><span data-stu-id="4d888-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="4d888-124">Giám sát việc tuân thủ thiết bị InTune</span><span class="sxs-lookup"><span data-stu-id="4d888-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="4d888-125">Lưu ý: các bước sau đây chỉ hữu ích trong việc khắc phục sự cố truy nhập các tính năng Azure Active Directory có điều kiện.</span><span class="sxs-lookup"><span data-stu-id="4d888-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="4d888-126">Cũng có thể để cách ly thiết bị chặn truy nhập email với chính sách Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d888-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="4d888-127">Tìm hiểu thêm thông tin về quản lý thiết bị Exchange [ở đây] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="4d888-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
