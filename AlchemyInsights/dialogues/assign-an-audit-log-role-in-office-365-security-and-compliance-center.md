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
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527558"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Gán vai trò kiểm tra Nhật ký trong Trung tâm tuân thủ & bảo mật của Office 365

Để tìm kiếm Nhật ký kiểm tra Office 365, người quản trị phải được gán vai trò **Nhật ký kiểm tra dạng xem** hoặc vai trò **Nhật ký kiểm** tra trong Exchange Online. Các vai trò này được gán cho nhóm vai trò quản lý tuân thủ và quản lý tổ chức theo mặc định. Người quản trị toàn cầu trong Office 365 và Microsoft 365 sẽ tự động được thêm vào như là thành viên của nhóm vai trò quản lý tổ chức.

Để cho phép người dùng tìm kiếm với mức đặc quyền tối thiểu, hãy tạo nhóm vai trò tùy chỉnh trong Exchange Online, thêm vai trò **Nhật ký kiểm tra chỉ xem** hoặc vai trò **Nhật ký kiểm** nghiệm, sau đó thêm người dùng dưới dạng thành viên của nhóm vai trò mới.

Để biết thêm thông tin, hãy xem [quản lý nhóm vai trò trong Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) và [Tìm kiếm Nhật ký kiểm tra trong Trung tâm tuân thủ & bảo mật](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).