---
title: Không thể xoá các mục trong SharePoint hoặc OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36748598"
---
# <a name="unable-to-delete-items"></a>Không thể xoá các mục

Có vấn đề xóa các mục SharePoint?

- Luôn đảm bảo rằng bạn có quyền [thích hợp](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) để xoá mục hoặc có một [quản trị viên bộ sưu tập trang web](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) cố gắng loại bỏ mục.

- Đảm bảo rằng không có thiết lập [chính sách lưu giữ](https://docs.microsoft.com/office365/securitycompliance/retention-policies) trên mục.

- Đảm bảo mục không được [kiểm tra](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) cho người dùng khác.

- Cuối cùng, quản trị viên có thể sử dụng [SharePoint Patterns và thực tiễn](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) chứa một thư viện lệnh PowerShell cho phép bạn thực hiện các hành động quản lý phức tạp như lực xóa các mục cứng đầu.
- [Loại bỏ PNP file](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Loại bỏ PNP cặp](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Loại bỏ PNP danh mục](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Loại bỏ PNP danh sách](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Loại bỏ PNP trường (cột)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)