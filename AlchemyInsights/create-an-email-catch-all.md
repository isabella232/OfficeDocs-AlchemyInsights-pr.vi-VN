---
title: Tạo email để nắm bắt tất cả
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080768"
---
# <a name="create-an-email-catch-all"></a>Tạo email để nắm bắt tất cả

Bạn không nên sử dụng tính năng bắt kịp tất cả. Tốt hơn là nên trả lại thư cho người gửi để cho người gửi biết thư của họ không thể được chuyển phát như đã được giải quyết để họ có thể hành động. Bạn cũng có thể giới hạn hộp thư được theo dõi chỉ nắm được địa chỉ email hợp lệ trước đây. 

Mọi lưu lượng hộp thư đều sẽ nhận được một loại thư rác tốt và cuối cùng có thể sẽ điền vào nếu không được theo dõi chặt chẽ. (Có giới hạn nhận được.) 

Nếu bạn quyết định tiếp tục, hãy làm theo các bước sau:

1. Tạo Nhóm Phân phối Động để & gồm "Tất cả Các Loại Người nhận".

2. Tạo một Hộp thư chuyên dụng để nắm bắt các email, ví dụ như email catchall@domain.com.

3. Đối với miền cụ thể, hãy đặt DomainType thành "InternalRelay". Nếu sau đó bạn loại bỏ tất cả, hãy đảm bảo đặt miền trở lại là Có thẩm quyền.

4. Tạo Quy tắc Truyền dẫn Dòng thư như sau:

    - Nếu Người gửi là "Bên ngoài Tổ chức"
    - Chuyển hướng thư đến Catchall@domain.com
    - Ngoại trừ nếu người nhận là thành viên của allusers@domain.com (Nhóm Phân phối chứa tất cả các thành viên)
    - Đảm bảo xác thực rằng các hộp thư mới được thêm vào Nhóm Phân phối Động
