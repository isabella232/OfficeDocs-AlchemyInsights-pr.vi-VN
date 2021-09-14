---
title: Báo cáo trong Trung tâm quản trị Microsoft 365 không hiển thị tên người dùng có thể đọc
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2021
ms.locfileid: "59316356"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Báo cáo trong Trung tâm quản trị Microsoft 365 không hiển thị tên người dùng có thể đọc

Báo cáo trong Trung tâm quản trị Microsoft 365 không hiển thị tên người dùng mà thay vào đó hiển thị các giá trị chữ và số như B2BC6C15BB9FCDEA71E5CD302D228CC8.

Đây là hành vi dự kiến và đã được thông báo trong Trung tâm Thông báo (MC275344, phát hành vào 03/08/2021). 

Người quản trị toàn cầu có thể hoàn nguyên thay đổi này cho đối tượng thuê của họ và hiển thị thông tin người dùng có thể nhận dạng nếu các thực hành về quyền riêng tư của tổ chức của họ cho phép. Để hoàn nguyên thay đổi cho đối tượng thuê:

1. Trong trung tâm quản trị, đi đến **cài Cài đặt** Dịch vụ cài  >  **đặt tổ**  >  [**chức**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services), rồi chọn Báo **cáo**. 
1. Bên **dưới Mục Chọn cách hiển** thị thông tin người dùng, chọn Hiển thị thông tin người dùng có thể nhận dạng trong báo cáo , rồi chạy lại báo cáo. 