---
title: Gán vai trò kiểm tra Nhật ký trong Trung tâm tuân thủ & bảo mật của Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749528"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="972ca-102">Gán vai trò kiểm tra Nhật ký trong Trung tâm tuân thủ & bảo mật của Office 365</span><span class="sxs-lookup"><span data-stu-id="972ca-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="972ca-103">Để tìm kiếm Nhật ký kiểm tra Office 365, người quản trị phải được gán vai trò **Nhật ký kiểm tra dạng xem** hoặc vai trò **Nhật ký kiểm** tra trong Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="972ca-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="972ca-104">Các vai trò này được gán cho nhóm vai trò quản lý tuân thủ và quản lý tổ chức theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="972ca-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="972ca-105">Người quản trị toàn cầu trong Office 365 và Microsoft 365 sẽ tự động được thêm vào như là thành viên của nhóm vai trò quản lý tổ chức.</span><span class="sxs-lookup"><span data-stu-id="972ca-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="972ca-106">Để cho phép người dùng tìm kiếm với mức đặc quyền tối thiểu, hãy tạo nhóm vai trò tùy chỉnh trong Exchange Online, thêm vai trò **Nhật ký kiểm tra chỉ xem** hoặc vai trò **Nhật ký kiểm** nghiệm, sau đó thêm người dùng dưới dạng thành viên của nhóm vai trò mới.</span><span class="sxs-lookup"><span data-stu-id="972ca-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="972ca-107">Để biết thêm thông tin, hãy xem [quản lý nhóm vai trò trong Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) và [Tìm kiếm Nhật ký kiểm tra trong Trung tâm tuân thủ & bảo mật](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="972ca-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>