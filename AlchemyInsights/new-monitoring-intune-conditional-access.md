---
title: Theo dõi quyền truy nhập InTune có điều kiện
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428312"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="b6c04-102">Theo dõi quyền truy nhập InTune có điều kiện</span><span class="sxs-lookup"><span data-stu-id="b6c04-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="b6c04-103">Người dùng được mục tiêu với quyền truy nhập có điều kiện sẽ nhận được email thông báo nếu họ không đáp ứng các yêu cầu truy nhập của tổ chức bạn.</span><span class="sxs-lookup"><span data-stu-id="b6c04-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="b6c04-104">Để giải quyết, chúng tôi khuyên bạn nên một hoặc nhiều giải pháp sau đây:</span><span class="sxs-lookup"><span data-stu-id="b6c04-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="b6c04-105">Nếu thiết bị được cho là đã đăng ký, hãy tư vấn cho người dùng để đi đến ứng dụng cổng thông tin công ty và xác minh rằng nó sẽ xuất hiện trong cổng thông tin công ty.</span><span class="sxs-lookup"><span data-stu-id="b6c04-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="b6c04-106">Nếu không, người dùng phải đăng ký thiết bị.</span><span class="sxs-lookup"><span data-stu-id="b6c04-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="b6c04-107">Trong cổng thông tin Azure, đi đến  >  **tuân thủ thiết bị** InTune.</span><span class="sxs-lookup"><span data-stu-id="b6c04-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="b6c04-108">Để xem báo cáo tuân thủ thiết bị của bạn để xác minh rằng thiết bị của người dùng được đánh dấu là tuân thủ, bên dưới **giám sát**, hãy bấm **tuân thủ thiết bị**.</span><span class="sxs-lookup"><span data-stu-id="b6c04-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="b6c04-109">Trong cổng thông tin Azure, đi đến  >  **tuân thủ thiết bị** InTune.</span><span class="sxs-lookup"><span data-stu-id="b6c04-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="b6c04-110">Bên dưới **quản lý,** bấm vào **chính sách**.</span><span class="sxs-lookup"><span data-stu-id="b6c04-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="b6c04-111">Trong danh sách các chính sách tuân thủ, hãy xác nhận hồ sơ được gán cho thiết bị của người dùng.</span><span class="sxs-lookup"><span data-stu-id="b6c04-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="b6c04-112">Nếu không có hồ sơ nào được phân công, thì InTune sẽ không thể xác nhận trạng thái tuân thủ của thiết bị.</span><span class="sxs-lookup"><span data-stu-id="b6c04-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="b6c04-113">Chỉnh sửa nhiệm vụ truy nhập có điều kiện của người dùng.</span><span class="sxs-lookup"><span data-stu-id="b6c04-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="b6c04-114">Trong cổng thông tin Azure, dẫn hướng đến các chính sách truy nhập **InTune** có điều  >  **kiện**  >  , hãy chọn một chính sách từ danh sách và bấm vào **người dùng và nhóm**.</span><span class="sxs-lookup"><span data-stu-id="b6c04-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="b6c04-115">Để nhắm đến một chính sách nhất định tại một ai đó, hãy thêm họ vào **danh sách bao gồm**.</span><span class="sxs-lookup"><span data-stu-id="b6c04-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="b6c04-116">Để đảm bảo rằng một người được bỏ qua khỏi chính sách, hãy thêm họ vào **danh sách loại trừ**.</span><span class="sxs-lookup"><span data-stu-id="b6c04-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="b6c04-117">**Liên kết hữu ích:**</span><span class="sxs-lookup"><span data-stu-id="b6c04-117">**Helpful links:**</span></span>

- [<span data-ttu-id="b6c04-118">Tổng quan về tuân thủ thiết bị</span><span class="sxs-lookup"><span data-stu-id="b6c04-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="b6c04-119">Khắc phục sự cố</span><span class="sxs-lookup"><span data-stu-id="b6c04-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="b6c04-120">Chính sách khắc phục sự cố</span><span class="sxs-lookup"><span data-stu-id="b6c04-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="b6c04-121">Giám sát việc tuân thủ thiết bị InTune</span><span class="sxs-lookup"><span data-stu-id="b6c04-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="b6c04-122">Các bước này chỉ hữu ích trong việc khắc phục sự cố truy nhập các tính năng Azure Active Directory có điều kiện.</span><span class="sxs-lookup"><span data-stu-id="b6c04-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="b6c04-123">Cũng có thể để cách ly thiết bị chặn truy nhập email với chính sách Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6c04-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="b6c04-124">Có thể tìm hiểu thêm thông tin về quản lý thiết bị Exchange [**tại đây**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span><span class="sxs-lookup"><span data-stu-id="b6c04-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
