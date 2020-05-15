---
title: Di chuyển từ AIP sang MIP/ghi nhãn hợp nhất trong Trung tâm tuân thủ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7ce9c387fc94f59674a922c5fe071fc0fb030344
ms.sourcegitcommit: e6d73d240669342fde9d4d25b0ee2838b7e43965
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/14/2020
ms.locfileid: "44236563"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="a1c74-102">Di chuyển từ AIP sang MIP/ghi nhãn hợp nhất trong Trung tâm tuân thủ</span><span class="sxs-lookup"><span data-stu-id="a1c74-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="a1c74-103">Để di chuyển từ nhãn AIP sang ghi nhãn hợp nhất trong Trung tâm bảo mật và tuân thủ, hãy làm như sau:</span><span class="sxs-lookup"><span data-stu-id="a1c74-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="a1c74-104">**Kích hoạt bảo vệ từ cổng Azure**</span><span class="sxs-lookup"><span data-stu-id="a1c74-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="a1c74-105">Nếu bạn chưa làm như vậy, hãy mở cửa sổ trình duyệt mới và [đăng nhập vào cổng thông tin Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="a1c74-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="a1c74-106">Điều hướng đến lưỡi **bảo vệ thông tin Azure** .</span><span class="sxs-lookup"><span data-stu-id="a1c74-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="a1c74-107">Ví dụ: trên menu Trung tâm, bấm vào **tất cả các dịch vụ** và bắt đầu nhập **thông tin** trong hộp lọc.</span><span class="sxs-lookup"><span data-stu-id="a1c74-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="a1c74-108">Chọn **bảo vệ thông tin Azure**.</span><span class="sxs-lookup"><span data-stu-id="a1c74-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="a1c74-109">Nếu bạn chưa truy cập lưỡi bảo vệ thông tin Azure trước đó, hãy xem các [bước bổ sung](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) một lần để thêm lưỡi này vào cổng thông tin.</span><span class="sxs-lookup"><span data-stu-id="a1c74-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="a1c74-110">Để mở lưỡi bảo vệ thông tin Azure, bạn phải có [gói Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) hoặc gói Office 365 bao gồm quản lý quyền.</span><span class="sxs-lookup"><span data-stu-id="a1c74-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="a1c74-111">Nếu bạn có một trong các mục đăng ký nhưng thấy thông báo rằng đăng ký hợp lệ không thể tìm thấy, hãy [liên hệ với Microsoft support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) hoặc sử dụng kênh hỗ trợ tiêu chuẩn của bạn.</span><span class="sxs-lookup"><span data-stu-id="a1c74-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="a1c74-112">Tìm tùy chọn **quản lý** menu và chọn **kích hoạt bảo vệ**.</span><span class="sxs-lookup"><span data-stu-id="a1c74-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="a1c74-113">Bấm **kích hoạt**, và sau đó xác nhận hành động của bạn.</span><span class="sxs-lookup"><span data-stu-id="a1c74-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="a1c74-114">Khi kích hoạt hoàn tất, thanh thông tin hiển thị **kích hoạt hoàn tất thành công**.</span><span class="sxs-lookup"><span data-stu-id="a1c74-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="a1c74-115">**Di chuyển Azure bảo vệ thông tin nhãn cho Office 365 bảo mật & Trung tâm tuân thủ**</span><span class="sxs-lookup"><span data-stu-id="a1c74-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="a1c74-116">Đảm bảo rằng bạn đã đăng nhập người dùng với quyền quản trị toàn cầu.</span><span class="sxs-lookup"><span data-stu-id="a1c74-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="a1c74-117">Điều hướng đến lưỡi **bảo vệ thông tin Azure** .</span><span class="sxs-lookup"><span data-stu-id="a1c74-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="a1c74-118">Từ tùy chọn **quản lý** menu, chọn **ghi nhãn hợp nhất**.</span><span class="sxs-lookup"><span data-stu-id="a1c74-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="a1c74-119">Trên **Azure thông tin bảo vệ-hợp nhất nhãn** Blade, bấm **kích hoạt** và làm theo hướng dẫn trực tuyến.</span><span class="sxs-lookup"><span data-stu-id="a1c74-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="a1c74-120">**Lưu ý**: xác minh rằng bạn có quyền thích hợp trước khi kích hoạt di chuyển trung tâm tuân thủ & bảo mật.</span><span class="sxs-lookup"><span data-stu-id="a1c74-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="a1c74-121">Xem các bài viết này để biết thêm thông tin:</span><span class="sxs-lookup"><span data-stu-id="a1c74-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="a1c74-122">Bạn có cần phải là quản trị viên toàn cầu để cấu hình bảo vệ thông tin Azure hoặc tôi có thể ủy nhiệm cho các quản trị viên khác không?</span><span class="sxs-lookup"><span data-stu-id="a1c74-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="a1c74-123">Thông tin quan trọng về vai trò quản trị sau khi di chuyển sang bảo mật & tuân thủ trung tâm.</span><span class="sxs-lookup"><span data-stu-id="a1c74-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="a1c74-124">Để biết thêm thông tin về AIP để di chuyển ghi nhãn hợp nhất vào Trung tâm bảo mật và tuân thủ, hãy xem [di chuyển nhãn](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="a1c74-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
