---
title: Sử dụng trang web Wix với Office 365 tên miền được mua hoặc quản lý
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: d7df06d768eabb44bcaee4a7450d16ecdb3395da4cee4810503d3dae358736ab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53980199"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Sử dụng trang web Wix với Office 365 tên miền được mua hoặc quản lý

- [Cập nhật bản ghi DNS để tiếp tục lưu trữ website tại nhà cung cấp lưu trữ hiện tại của bạn](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Bài viết "Connecting a Domain to Wix Using the Pointing Method" của Wix khuyên bạn nên sử dụng phương pháp trỏ (thêm bản ghi DNS cho mỗi liên kết bên trên) thay vì thay đổi máy chủ tên khi sử dụng Office 365
- Nếu bạn vẫn chọn thay đổi máy chủ tên thành Wix, bạn sẽ cần Tạo bản ghi  [DNS tại Wix cho Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Nếu bạn mua miền từ Microsoft thì không thể thay đổi tên miền. Nếu bạn phải thay đổi tên máy chủ, miền do Microsoft mua sẽ cần phải được chuyển sang nhà cung cấp  [lưu trữ khác sau 60 ngày](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)