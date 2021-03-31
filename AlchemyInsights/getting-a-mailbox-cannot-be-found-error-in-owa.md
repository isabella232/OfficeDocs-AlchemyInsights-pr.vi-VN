---
title: 126 nhận được một hộp thư không thể tìm thấy lỗi trong OWA?
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
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426684"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Bạn nhận được một hộp thư không tìm thấy lỗi trong Outlook trên web?

Nếu bạn đang sử dụng Outlook trên web và bạn nhận được một **hộp thư không thể tìm thấy** được lỗi, tài khoản mà bạn đã sử dụng để kết nối với Outlook trên web không có giấy phép Exchange Online và do đó, không có hộp thư nào được liên kết với tài khoản đó. Người quản trị có thể gán giấy phép cho tài khoản của bạn bằng cách làm theo các bước sau đây:

1. Mở [Trung tâm quản trị Microsoft 365](https://portal.office.com/adminportal/home#/homepage) và đi tới **người dùng hiện hoạt** bên dưới mục **người dùng** , rồi chọn người dùng đang nhìn thấy lỗi.

2. Trong trang người dùng mở ra, hãy đi đến phần **giấy phép và ứng dụng** , chọn giá trị **vị trí** thích hợp và gán giấy phép có chứa Exchange Online (bung rộng giấy phép để xem chi tiết của nó). Khi bạn đã hoàn tất, hãy bấm **lưu thay đổi**.

Trong một số trường hợp, nếu giấy phép đã được gán cho một tài khoản người dùng, hãy loại bỏ và gán lại giấy phép sẽ giúp giải quyết sự cố này và nhận được quyền được cung cấp đúng cách trong hệ thống: 

- Kiểm tra xem liệu M365 Exchange Online của bạn (và khác, nếu bạn có bất kỳ thuê bao nào) hiện tại và chưa hết hạn.

Sau khi bạn đã đảm bảo rằng đăng ký của bạn đã không hết hạn và một giấy phép hợp lệ đã được gán cho tài khoản người dùng, có thể mất đến 24 giờ để được cung cấp để được cung cấp, vì vậy bạn có thể phải đợi vấn đề của bạn để giải quyết. Để biết thêm thông tin, hãy xem mục [gán và quản lý giấy phép](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).