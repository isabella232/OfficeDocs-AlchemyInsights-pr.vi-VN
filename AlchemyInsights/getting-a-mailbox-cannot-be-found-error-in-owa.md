---
title: 126 Không thể tìm thấy lỗi Nhận hộp thư trong OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: aca0371dad9ba43fa21b0df8e50f1b8ee536528af90d6bda401995c6e5796be4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056512"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Không tìm thấy lỗi nhận được hộp thư trong Outlook trên web?

Nếu bạn đang sử dụng Outlook trên web và  gặp phải Không thể tìm thấy Hộp thư do lỗi nên tài khoản bạn đã sử dụng để kết nối với Outlook trên web không có giấy phép Exchange Online và do đó, không có hộp thư nào được liên kết với tài khoản đó. Người quản trị có thể gán giấy phép cho tài khoản của bạn bằng cách làm theo các bước sau:

1. Mở hộp [Trung tâm quản trị Microsoft 365](https://portal.office.com/adminportal/home#/homepage) rồi đi tới Người  **dùng hiện hoạt** bên dưới mục Người dùng, rồi chọn người dùng gặp phải lỗi.

2. Trong trang người dùng mở ra, đi đến mục Giấy  phép và Ứng dụng, chọn giá trị Vị trí thích hợp, rồi gán giấy phép có chứa Exchange Online (bung rộng giấy phép để xem chi tiết).  Khi bạn hoàn tất, hãy bấm Lưu **thay đổi**.

Trong một số trường hợp, nếu giấy phép đã được gán cho một tài khoản người dùng, việc loại bỏ và gán lại giấy phép sẽ giúp giải quyết sự cố và cung cấp đúng cách giấy phép trong hệ thống: 

- Kiểm tra xem đăng ký M365 Exchange Online (và các đăng ký khác, nếu bạn có) có đăng ký hiện thời hay chưa và chưa hết hạn gần đây.

Sau khi bạn đã đảm bảo rằng đăng ký của mình chưa hết hạn và giấy phép hợp lệ đã được gán cho tài khoản người dùng, có thể mất đến 24 giờ để giấy phép được cung cấp, vì vậy có thể bạn phải chờ vấn đề của mình giải quyết. Để biết thêm thông tin, hãy [xem Gán và quản lý giấy phép](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).