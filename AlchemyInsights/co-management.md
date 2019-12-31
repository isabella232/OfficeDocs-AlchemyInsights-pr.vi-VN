---
title: Đồng quản lý
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: fe7dcebf847fbd7d91632e93e2253bf62ac659aa
ms.sourcegitcommit: 4ed431b2e1aed26d07bd7eba282531537d29ad0e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/30/2019
ms.locfileid: "40910506"
---
# <a name="co-management"></a><span data-ttu-id="9d70a-102">Đồng quản lý</span><span class="sxs-lookup"><span data-stu-id="9d70a-102">Co-management</span></span>

<span data-ttu-id="9d70a-103">**Điều kiện tiên quyết để di chuyển từ config Manager Hybrid InTune**</span><span class="sxs-lookup"><span data-stu-id="9d70a-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="9d70a-104">Đánh giá [bài viết này](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span><span class="sxs-lookup"><span data-stu-id="9d70a-104">Review [this article](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span></span>
- <span data-ttu-id="9d70a-105">[Thêm một giấy phép InTune cho người dùng của bạn](https://docs.microsoft.com/intune/licenses-assign).</span><span class="sxs-lookup"><span data-stu-id="9d70a-105">[Add an Intune license to your users](https://docs.microsoft.com/intune/licenses-assign).</span></span>
- <span data-ttu-id="9d70a-106">Sử dụng [trình duyệt Edge](https://www.microsoft.com/windows/microsoft-edge) khi cấu hình đồng quản lý.</span><span class="sxs-lookup"><span data-stu-id="9d70a-106">Use the [Edge browser](https://www.microsoft.com/windows/microsoft-edge) when configuring Co-management.</span></span>

<span data-ttu-id="9d70a-107">**Làm thế nào để cài đặt máy khách quản lý cấu hình trên thiết bị quản lý InTune**</span><span class="sxs-lookup"><span data-stu-id="9d70a-107">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="9d70a-108">Xem [các thiết bị Windows quản lý MDM](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span><span class="sxs-lookup"><span data-stu-id="9d70a-108">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="9d70a-109">**Điều gì nếu tôi chỉ muốn thay đổi quyền MDM?**</span><span class="sxs-lookup"><span data-stu-id="9d70a-109">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="9d70a-110">Cơ quan MDM có thể thay đổi mà không cần mở một trường hợp hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="9d70a-110">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="9d70a-111">Vui lòng đánh giá các tài liệu sau để hỗ trợ thay đổi quyền MDM:</span><span class="sxs-lookup"><span data-stu-id="9d70a-111">Please review the following documentation to assist in changing your MDM authority:</span></span>
- [<span data-ttu-id="9d70a-112">Thay đổi quyền MDM từ config quản lý để InTune độc lập</span><span class="sxs-lookup"><span data-stu-id="9d70a-112">Change MDM Authority from Config Manager to Intune standalone</span></span>](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-change-mdm-authority)
- [<span data-ttu-id="9d70a-113">Thay đổi quyền MDM từ InTune độc lập để quản lý cấu hình</span><span class="sxs-lookup"><span data-stu-id="9d70a-113">Change MDM Authority from Intune standalone to Config Manager</span></span>](https://docs.microsoft.com/intune-classic/deploy-use/prerequisites-for-enrollment#what-to-do-if-you-choose-the-wrong-mdm-authority-setting)