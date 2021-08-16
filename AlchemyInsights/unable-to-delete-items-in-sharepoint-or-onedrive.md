---
title: Không thể xóa các mục trong SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038539"
---
# <a name="unable-to-delete-items"></a>Không thể xóa các mục

- Chính sách duy trì có thể gây ra vấn đề này, bạn cần tắt hoặc loại trừ việc giữ tương ứng đang gây ra vấn đề này. Sau khi chính sách duy trì hoặc giữ bị loại bỏ, có thể mất đến 24 giờ để thay đổi có hiệu lực. Đảm bảo rằng không có thiết lập [chính sách](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) duy trì trên mục.

- Site có thể đã vượt quá giới hạn lưu trữ, tăng [hạn mức site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) và xóa mục.

- Đảm bảo mục không được [kiểm xuất cho](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) người dùng khác.

- Cuối cùng, người quản trị có thể sử dụng Mẫu hình và Thực hành (PnP) [SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) có chứa thư viện các lệnh PowerShell cho phép bạn thực hiện các hành động quản lý phức tạp như bắt buộc xóa các mục stub gửi đi.
- [Loại bỏ Tệp PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Loại bỏ Thư mục PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Loại bỏ Mục Danh sách PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Loại bỏ Danh sách PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Loại bỏ Trường PNP (Cột)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)