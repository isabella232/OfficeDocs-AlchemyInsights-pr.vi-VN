---
title: Ảnh người dùng vẫn xuất hiện trong sơ đồ Microsoft Teams tổ chức
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422313"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Ảnh người dùng vẫn xuất hiện trong sơ đồ Microsoft Teams tổ chức

Nếu một hoặc nhiều cá nhân trong tổ chức của bạn đã bị vô hiệu hóa hoặc loại bỏ và ảnh hồ sơ của họ vẫn xuất hiện trong sơ đồ tổ chức thì có thể thiết đặt **ShowInAddressLists** được đặt thành False: 

1. Đi tới Trung tâm quản trị Microsoft 365 > [người dùng Hiện](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) hoạt và chọn người dùng có ảnh vẫn xuất hiện. 
1. Chọn tab **Thư** và đảm bảo Hiển thị **trong danh sách địa chỉ toàn cầu** được đặt là **Không.**

Nếu việc **đặt ShowInAddressLists** thành **No** không hoạt động, hãy kiểm tra các mục sau: 

- Người dùng có thể được hiển thị từ danh sách người nhận trong Exchange. Để biết thêm thông tin, hãy [xem mục Quản lý danh sách địa chỉ Exchange Online.](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- Người dùng có thể được hiển thị từ danh sách địa chỉ trong Azure Active Directory. Để biết thêm thông tin, [hãy xem Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 