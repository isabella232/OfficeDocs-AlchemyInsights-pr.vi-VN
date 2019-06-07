---
title: Không thể xoá mục trong SharePoint hoặc OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 82a19c8ea218834b71901e95747da0c99243893e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757946"
---
# <a name="unable-to-delete-items"></a>Không thể xoá bỏ khoản mục

Có vấn đề xóa mục?

- Luôn chắc chắn rằng bạn có [quyền phù hợp](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) để xóa mục hoặc có một [bộ sưu tập quản lý](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) cố gắng loại bỏ các mục.

- Đảm bảo rằng có không phải là một thiết lập [chính sách lưu giữ](https://docs.microsoft.com/office365/securitycompliance/retention-policies) trên mặt hàng đó.

- Bảo đảm hàng không [kiểm tra](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) đến người dùng khác.

- Cuối cùng, người quản trị có thể sử dụng [SharePoint Patterns và thực tiễn](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) chứa một thư viện của PowerShell lệnh cho phép bạn thực hiện các hoạt động quản lý phức tạp như buộc xóa mục bướng bỉnh. 
- [Loại bỏ tệp PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Loại bỏ cặp PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Loại bỏ các mục danh sách PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Xoá danh sách PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Loại bỏ các PNP trường (cột)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)