---
title: Tạo nhóm
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089181"
---
# <a name="create-a-group"></a><span data-ttu-id="7d70f-102">Tạo nhóm</span><span class="sxs-lookup"><span data-stu-id="7d70f-102">Create a group</span></span>

<span data-ttu-id="7d70f-103">Chủ đề này mô tả việc tạo nhóm.</span><span class="sxs-lookup"><span data-stu-id="7d70f-103">This topic describes group creation.</span></span>

<span data-ttu-id="7d70f-104">**Quyền tạo nhóm**</span><span class="sxs-lookup"><span data-stu-id="7d70f-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="7d70f-105">Đảm bảo bạn được ủy quyền để tạo nhóm mới.</span><span class="sxs-lookup"><span data-stu-id="7d70f-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="7d70f-106">Người quản trị toàn cầu có thể tắt tính năng tạo nhóm trong cổng thông tin Azure hoặc Pa-nen truy nhập.</span><span class="sxs-lookup"><span data-stu-id="7d70f-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="7d70f-107">Bạn có thể cần người quản trị để tạo nhóm mới cho bạn hoặc để cung cấp cho bạn quyền thích hợp.</span><span class="sxs-lookup"><span data-stu-id="7d70f-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="7d70f-108">**Quản lý quyền tạo nhóm**</span><span class="sxs-lookup"><span data-stu-id="7d70f-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="7d70f-109">Người quản trị toàn cầu có thể quản lý quyền tạo nhóm (cho các lý do liên quan đến bảo mật) hoặc các nhóm Office 365 được tạo trong Azure Portal hoặc Access Panel, bằng cách chọn "người dùng có thể tạo nhóm bảo mật trong Azure Portals" hoặc "người dùng có thể tạo nhóm Office 365 trong Azure Portals" tùy chọn trong **tất cả các nhóm**  >  **chung (thiết đặt)**</span><span class="sxs-lookup"><span data-stu-id="7d70f-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="7d70f-110">Bạn cũng có thể hạn chế tạo nhóm để chọn một nhóm người dùng nếu bạn có giấy phép Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="7d70f-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="7d70f-111">**Tắt thông báo chào mừng cho các thành viên nhóm mới của Office 365**</span><span class="sxs-lookup"><span data-stu-id="7d70f-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="7d70f-112">Thông báo chào mừng được gửi đến những người dùng được thêm vào các nhóm Office 365 có thể bị vô hiệu hóa bằng cách đặt **Unifiedgroupwelcomemessageenabled** thành false trong PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7d70f-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="7d70f-113">Tìm hiểu về thiết đặt này [ở đây](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="7d70f-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

