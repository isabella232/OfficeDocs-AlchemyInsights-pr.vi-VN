---
title: Đồng bộ hóa nhóm
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256912"
---
# <a name="group-sync"></a><span data-ttu-id="545dc-102">Đồng bộ hóa nhóm</span><span class="sxs-lookup"><span data-stu-id="545dc-102">Group sync</span></span>

<span data-ttu-id="545dc-103">Bài viết này cung cấp hướng dẫn về đồng bộ hóa nhóm.</span><span class="sxs-lookup"><span data-stu-id="545dc-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="545dc-104">Nếu người quản trị toàn cầu hoặc chủ sở hữu nhóm không thể sửa đổi thuộc tính nhóm hoặc thêm thành viên hoặc gán chủ sở hữu trong cổng thông tin Azure, hãy đảm bảo nguồn của chính quyền cho nhóm là Azure Active Directory (Azure AD) cho người quản trị toàn cầu hoặc chủ sở hữu nhóm để sửa đổi nhóm.</span><span class="sxs-lookup"><span data-stu-id="545dc-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="545dc-105">Trước khi tìm cách xóa một nhóm đã đồng bộ trong Azure AD, hãy đảm bảo rằng bạn đã [xóa tất cả giấy phép đã gán](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) để tránh lỗi.</span><span class="sxs-lookup"><span data-stu-id="545dc-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="545dc-106">Để biết cách đồng bộ hóa người dùng, nhóm và liên hệ, hãy xem [AZURE AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)và theo dõi đồng bộ [một nhóm tại chỗ để AZURE bằng Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) để đồng bộ trên hình uốn nhóm bằng cách sử dụng kết nối quảng cáo.</span><span class="sxs-lookup"><span data-stu-id="545dc-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="545dc-107">Hãy làm theo các [lỗi khắc phục sự cố hướng dẫn này trong quá trình đồng bộ](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) để khắc phục các lỗi thường gặp</span><span class="sxs-lookup"><span data-stu-id="545dc-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

