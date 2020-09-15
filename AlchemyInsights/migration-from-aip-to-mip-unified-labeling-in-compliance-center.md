---
title: Di chuyển từ AIP đến MIP/ghi nhãn hợp nhất trong Trung tâm tuân thủ
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674348"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="6d662-102">Di chuyển từ AIP đến MIP/ghi nhãn hợp nhất trong Trung tâm tuân thủ</span><span class="sxs-lookup"><span data-stu-id="6d662-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="6d662-103">Để di chuyển từ nhãn AIP để ghi nhãn hợp nhất trong Trung tâm bảo mật và tuân thủ, hãy thực hiện như sau:</span><span class="sxs-lookup"><span data-stu-id="6d662-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="6d662-104">**Kích hoạt bảo vệ từ cổng thông tin Azure**</span><span class="sxs-lookup"><span data-stu-id="6d662-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="6d662-105">Nếu bạn chưa làm như vậy, hãy mở một cửa sổ trình duyệt mới và [đăng nhập vào cổng thông tin Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="6d662-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="6d662-106">Dẫn hướng đến lưỡi dao **bảo vệ thông tin Azure** .</span><span class="sxs-lookup"><span data-stu-id="6d662-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="6d662-107">Ví dụ, trên menu Hub, bấm vào **tất cả dịch vụ** và bắt đầu nhập **thông tin** trong hộp bộ lọc.</span><span class="sxs-lookup"><span data-stu-id="6d662-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="6d662-108">Chọn **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="6d662-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="6d662-109">Nếu bạn chưa truy nhập vào lưỡi trước khi bảo vệ thông tin Azure, hãy xem các [bước bổ sung](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) một lần để thêm lưỡi dao này vào cổng thông tin.</span><span class="sxs-lookup"><span data-stu-id="6d662-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="6d662-110">Để mở các lưỡi dao bảo vệ thông tin Azure, bạn phải có một [gói bảo vệ thông tin Azure](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) hoặc gói Office 365 bao gồm quản lý quyền.</span><span class="sxs-lookup"><span data-stu-id="6d662-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="6d662-111">Nếu bạn có một trong các đăng ký này nhưng nhìn thấy thông báo rằng không tìm thấy một thuê bao hợp lệ, [hãy liên hệ với bộ phận](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) hỗ trợ của Microsoft hoặc dùng các kênh hỗ trợ tiêu chuẩn của bạn.</span><span class="sxs-lookup"><span data-stu-id="6d662-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="6d662-112">Xác định vị trí tùy chọn **quản lý** menu, rồi chọn **bảo vệ kích hoạt**.</span><span class="sxs-lookup"><span data-stu-id="6d662-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="6d662-113">Bấm **kích hoạt**, rồi xác nhận hành động của bạn.</span><span class="sxs-lookup"><span data-stu-id="6d662-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="6d662-114">Khi quá trình kích hoạt hoàn tất, thanh thông tin sẽ hiển thị việc **kích hoạt đã hoàn tất thành công**.</span><span class="sxs-lookup"><span data-stu-id="6d662-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="6d662-115">**Di chuyển nhãn bảo vệ thông tin Azure lên Trung tâm tuân thủ & bảo mật của Office 365**</span><span class="sxs-lookup"><span data-stu-id="6d662-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="6d662-116">Hãy đảm bảo bạn đã đăng nhập với tư cách người dùng với quyền của người quản trị toàn cầu.</span><span class="sxs-lookup"><span data-stu-id="6d662-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="6d662-117">Dẫn hướng đến lưỡi dao **bảo vệ thông tin Azure** .</span><span class="sxs-lookup"><span data-stu-id="6d662-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="6d662-118">Từ tùy chọn **quản lý** menu, chọn **ghi nhãn hợp nhất**.</span><span class="sxs-lookup"><span data-stu-id="6d662-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="6d662-119">Trên thanh **bảo vệ thông tin Azure-** lưỡi cắt dán hợp nhất, hãy bấm **kích hoạt** và làm theo hướng dẫn trực tuyến.</span><span class="sxs-lookup"><span data-stu-id="6d662-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="6d662-120">**Lưu ý**: xác nhận rằng bạn có quyền thích hợp trước khi kích hoạt di chuyển trung tâm tuân thủ & bảo mật.</span><span class="sxs-lookup"><span data-stu-id="6d662-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="6d662-121">Xem các bài viết này để biết thêm thông tin:</span><span class="sxs-lookup"><span data-stu-id="6d662-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="6d662-122">Bạn có cần phải là người quản trị toàn cầu để cấu hình bảo vệ thông tin Azure hoặc tôi có thể đại diện cho các người quản trị khác không?</span><span class="sxs-lookup"><span data-stu-id="6d662-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="6d662-123">Thông tin quan trọng về các vai trò quản trị sau khi di chuyển sang Trung tâm tuân thủ & bảo mật.</span><span class="sxs-lookup"><span data-stu-id="6d662-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="6d662-124">Để biết thêm thông tin về việc di chuyển nhãn hiệu của AIP để được thống nhất sang Trung tâm bảo mật và tuân thủ, hãy xem [di chuyển nhãn](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="6d662-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
