---
title: Không thể xóa bỏ các mục trong SharePoint hoặc OneDrive
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
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019605"
---
# <a name="unable-to-delete-items"></a>Không thể xóa các mục

- Các chính sách duy trì có thể gây ra điều này, bạn cần tắt hoặc loại trừ giữ tương ứng đang gây ra sự cố này. Sau khi một chính sách duy trì hoặc giữ được loại bỏ, có thể mất tới 24 giờ để thay đổi có hiệu lực. Đảm bảo rằng không có thiết lập [chính sách duy trì](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) trên mục.

- Site có thể vượt quá giới hạn dung lượng lưu trữ, tăng [hạn ngạch trang](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) và xóa mục đó.

- Đảm bảo mục không được [kiểm](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) xuất cho một người dùng khác.

- Cuối cùng, người quản trị có thể sử dụng các [mẫu và thực hành SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) chứa một thư viện của các lệnh PowerShell cho phép bạn thực hiện các hành động quản lý phức tạp chẳng hạn như buộc xóa các mục bướng bỉnh.
- [Loại bỏ tệp PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Loại bỏ thư mục PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Loại bỏ mục danh sách PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Loại bỏ danh sách PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Loại bỏ trường PNP (cột)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)