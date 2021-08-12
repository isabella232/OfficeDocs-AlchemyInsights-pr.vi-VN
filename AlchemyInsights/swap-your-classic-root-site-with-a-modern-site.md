---
title: Hoán đổi site gốc Cổ điển của bạn với site Hiện đại
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 7209595f5cda9b31e53241d9d5696fa584ff5e5ab3d237aae28542bf7aec9398
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940841"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Hoán đổi site gốc Cổ điển của bạn với site Hiện đại

Nếu môi trường của bạn được thiết lập trước Tháng Tư 2019, bạn có thể thay đổi site gốc của mình thành một site hiện đại bằng cách sử dụng Microsoft PowerShell:

- Nếu bạn có một site khác mà bạn muốn dùng làm site gốc của mình, thì bạn có thể thay [thế (hoán đổi) site gốc](https://docs.microsoft.com/sharepoint/modern-root-site) bằng site gốc đó. 
    - Dùng [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) để hoán đổi vị trí của site với một site khác trong khi lưu trữ site gốc. Sẵn dùng cho cả Site Nhóm (không được kết nối với nhóm) và Site Liên lạc. 

- Các chức năng bổ sung sẽ sớm được giới thiệu, điều này sẽ cho phép bạn tiếp tục sử dụng nội dung trên site, nhưng chuyển đổi site hiện có thành site liên lạc. 
>[!Important]
>Các chức năng này sẽ được triển khai dần. Tiếp tục kiểm tra bản cập nhật của Trung tâm Thông báo. 

## <a name="known-issues-with-swapping-sites"></a>Sự cố đã biết với hoán đổi site

- Site đích có thể trả về lỗi "không tìm thấy" (HTTP 404) trong một khoảng thời gian ngắn.
- Cần phải nhận biết nội dung để cập nhật chỉ mục tìm kiếm. Không cần thực hiện bước thủ công - thao tác này sẽ được thực hiện tự động.
- Mọi thứ phụ thuộc vào nối kết "tĩnh" (chẳng hạn như Đồng bộ Tệp và OneNote) sẽ cần được sửa thủ công.
- Nếu site nguồn là site tin tức của tổ chức, hãy cập nhật URL. Tải danh sách tất cả các site tin tức của tổ chức.
- Project Có thể các site máy chủ cần được xác thực để đảm bảo rằng chúng vẫn được liên kết đúng.
