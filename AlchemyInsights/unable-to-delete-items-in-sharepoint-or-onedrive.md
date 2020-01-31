---
title: Không thể xoá các mục trong SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571293"
---
# <a name="unable-to-delete-items"></a>Không thể xoá các mục

Chính sách lưu giữ có thể gây ra điều này, bạn cần tắt hoặc loại trừ các giữ tương ứng gây ra vấn đề này. Sau khi chính sách lưu giữ hoặc giữ bị xóa, có thể mất đến 24 giờ để thay đổi có hiệu lực. Đảm bảo rằng không có thiết lập [chính sách lưu giữ](https://docs.microsoft.com/office365/securitycompliance/retention-policies) trên mục.

Trang web có thể vượt quá giới hạn lưu trữ, tăng [dung lượng trang web](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) và xoá mục.

Đảm bảo mục không được [kiểm tra](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) cho người dùng khác.

Cuối cùng, quản trị viên có thể sử dụng [SharePoint Patterns và thực tiễn](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) chứa một thư viện lệnh PowerShell cho phép bạn thực hiện các hành động quản lý phức tạp như lực xóa các mục cứng đầu.
- [Loại bỏ PNP file](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Loại bỏ PNP cặp](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Loại bỏ PNP danh mục](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Loại bỏ PNP danh sách](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Loại bỏ PNP trường (cột)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)