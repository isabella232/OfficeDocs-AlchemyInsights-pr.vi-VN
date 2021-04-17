---
title: Giải quyết lỗi đăng nhập nhóm AADSTS9000411
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
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822009"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Giải quyết lỗi đăng nhập nhóm AADSTS9000411

Khi đăng nhập vào Microsoft nhóm, bạn có thể nhận được lỗi: **xin lỗi, nhưng chúng tôi đang gặp sự cố với việc đăng nhập vào AADSTS9000411: yêu cầu đó không được định dạng đúng. Tham số "login_hint" bị trùng lặp.**

Để giải quyết sự cố này, vui lòng đảm bảo rằng khách hàng Microsoft nhóm của bạn được Cập Nhật. Để biết thêm thông tin về việc Cập Nhật máy khách của bạn, hãy xem [Cập nhật các nhóm Microsoft](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Nếu bạn không thể cập nhật máy khách của mình vì lý do nào đó, hãy đăng xuất khỏi máy khách sẽ xóa hầu hết các dữ liệu được lưu trong bộ đệm ẩn. Tuy nhiên, nếu bạn vẫn gặp sự cố sau khi đăng xuất/đăng nhập, hãy thoát khỏi nhóm và vui lòng xóa bộ đệm ẩn máy khách của bạn bằng cách thực hiện như sau:
1. Đóng nhóm Microsoft.
2. Đi đến:%AppData%\microsoft\nhóm và xóa tất cả các tệp.
3. Mở lại nhóm Microsoft.
