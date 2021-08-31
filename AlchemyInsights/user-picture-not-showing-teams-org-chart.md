---
title: Ảnh người dùng không hiển thị trong Microsoft Teams đồ tổ chức
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792891"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Ảnh người dùng không hiển thị trong Microsoft Teams đồ tổ chức

Nếu một hoặc nhiều cá nhân trong tổ chức của bạn thiếu ảnh hồ sơ của họ trong sơ đồ tổ chức, có thể thiết đặt **ShowInAddressLists** được đặt thành **False:**

1. Đi tới Trung tâm quản trị Microsoft 365 > [**Người dùng Hiện hoạt**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users), rồi chọn người dùng bị thiếu ảnh. 
1. Chọn tab **Thư** và đảm bảo Hiển thị **trong danh sách địa chỉ toàn cầu** được đặt thành **Có.** 

Nếu việc đặt **ShowInAddressLists** thành **Yes** không hoạt động, hãy kiểm tra các mục sau:

- Người dùng có thể bị ẩn khỏi danh sách người nhận trong Exchange. Để biết thêm thông tin, hãy [xem mục Quản lý danh sách địa chỉ Exchange Online.](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- Người dùng có thể bị ẩn khỏi danh sách địa chỉ trong Azure Active Directory. Để biết thêm thông tin, [hãy xem Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
