---
title: Gán nhóm cho vai trò Azure AD
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
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036262"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Gán nhóm cho vai trò Azure AD

Để gán một nhóm Azure AD có nguồn thẩm quyền trong Azure AD cho vai trò Azure AD, hãy thực hiện các bước sau đây:

1. Tạo nhóm mới - Để tạo một nhóm mới:

    a. Đăng nhập vào trung tâm quản trị Azure AD với người **quản trị vai trò đặc quyền hoặc quyền** của người quản **trị** toàn cầu.
    b. Chọn **Azure Active Directory > nhóm > Nhóm tất cả > Nhóm mới.**
    c. Tạo nhóm.

2. Gán vai trò cho nhóm trong quá trình tạo nhóm hoặc sau khi tạo nhóm.

    a. Để gán vai trò cho nhóm vào lúc tạo nhóm, bạn có thể bật nút bật tắt vai trò **Azure AD** cho nhóm, rồi tạo nhóm.
    b. Để gán vai trò cho nhóm sau khi tạo nhóm, dẫn hướng đến **tab** Vai trò được gán cho nhóm mới được tạo, rồi gán vai trò cho nhóm đó.  

**Quản lý tư cách thành viên của nhóm được gán vai trò Azure AD**

Để ngăn mức nâng cao đặc quyền, theo mặc định, chỉ có người quản trị vai trò có đặc quyền và người quản trị toàn cầu mới có thể sửa đổi tư cách thành viên của nhóm được gán vai trò. Tuy nhiên, họ có thể chọn giao chủ sở hữu cho một nhóm như vậy và ủy nhiệm nhiệm vụ này.

Để biết thêm chi tiết về việc gán các nhóm đám mây cho vai trò Azure AD, xem mục [Gán vai trò AD cho Nhóm Đám mây](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Để biết thêm chi tiết về cách khắc phục sự cố vai trò được gán cho nhóm điện toán đám mây, hãy xem mục [Khắc phục sự cố vai trò được gán cho các nhóm điện toán đám mây](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





