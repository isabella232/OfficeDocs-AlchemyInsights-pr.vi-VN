---
title: Khắc phục sự cố chủ sở hữu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901272"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="5d836-102">Khắc phục sự cố chủ sở hữu</span><span class="sxs-lookup"><span data-stu-id="5d836-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="5d836-103">Để khắc phục sự cố liên quan đến chủ sở hữu, hãy thực hiện các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="5d836-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="5d836-104">[Thêm hoặc thay đổi người quản trị đăng ký Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): nhóm Azure Active Directory (Azure AD) đều thuộc sở hữu và do người sở hữu nhóm quản lý.</span><span class="sxs-lookup"><span data-stu-id="5d836-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="5d836-105">Chủ sở hữu nhóm có thể là người dùng hoặc hiệu trưởng dịch vụ và có thể quản lý nhóm, bao gồm tư cách thành viên.</span><span class="sxs-lookup"><span data-stu-id="5d836-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="5d836-106">Chỉ những chủ sở hữu nhóm hiện có hoặc người quản trị nhóm có thể gán cho người sở hữu nhóm.</span><span class="sxs-lookup"><span data-stu-id="5d836-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="5d836-107">Người sở hữu nhóm không bắt buộc phải là thành viên của nhóm.</span><span class="sxs-lookup"><span data-stu-id="5d836-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="5d836-108">[Thêm hoặc thay đổi người quản trị đăng ký Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): bài viết này mô tả cách thêm hoặc thay đổi vai trò người quản trị cho người dùng bằng cách sử dụng Azure RBAC tại phạm vi thuê bao.</span><span class="sxs-lookup"><span data-stu-id="5d836-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="5d836-109">Sử dụng PowerShell để thêm chủ sở hữu nhóm hoặc chủ sở hữu ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="5d836-109">Use PowerShell to add a group owner or an application owner.</span></span>
