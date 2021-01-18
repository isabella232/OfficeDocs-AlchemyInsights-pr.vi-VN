---
title: Gán nhóm tới Azure AD Role
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885403"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Gán nhóm tới Azure AD Role

Để gán một nhóm Azure AD với nguồn chính quyền trong Azure AD thành vai trò Azure AD, hãy thực hiện các bước sau đây:

1. Tạo nhóm mới-để tạo nhóm mới:

    một. Đăng nhập vào Trung tâm quản trị Azure AD với **người quản trị vai trò đặc quyền** hoặc quyền **người quản trị toàn cầu** .
    b. Chọn **các nhóm > Azure Active Directory > tất cả các nhóm > nhóm mới**.
    c's. Tạo nhóm.

2. Gán vai trò cho nhóm trong khi tạo nhóm hoặc sau khi nhóm được tạo.

    một. Để gán vai trò cho nhóm tại thời điểm tạo nhóm, hãy chuyển đổi trên các **vai trò chuyển đổi AZURE AD có thể được gán cho nhóm** và tạo nhóm.
    b. Để gán vai trò cho nhóm sau khi đã được tạo, hãy dẫn hướng đến tab **vai trò được gán** cho nhóm mới được tạo và gán vai trò cho nhóm.  

**Quản lý tư cách thành viên của một nhóm được gán cho vai trò Azure AD**

Để ngăn không cho độ cao của đặc quyền, theo mặc định, chỉ người quản trị vai trò đặc quyền và người quản trị toàn cầu có thể sửa đổi tư cách thành viên của một nhóm được gán cho vai trò. Tuy nhiên, họ có thể chọn gán chủ sở hữu cho một nhóm và đại diện cho nhiệm vụ này.

Để biết thêm chi tiết về việc gán nhóm điện toán đám mây thành Azure vai trò, hãy xem mục [gán vai trò quảng cáo cho nhóm điện toán đám mây](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Để biết thêm chi tiết về các vai trò khắc phục sự cố được gán cho nhóm đám mây, hãy xem [khắc phục các vai trò được gán cho nhóm đám mây](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





