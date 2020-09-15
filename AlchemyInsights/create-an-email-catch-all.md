---
title: Tạo một email bắt tất cả
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713008"
---
# <a name="create-an-email-catch-all"></a>Tạo một email bắt tất cả

Sử dụng tất cả bắt được khuyến khích mạnh mẽ. Tốt hơn là nên cung cấp một bản phân phát trở lại người gửi cho phép người gửi biết thư của họ không thể chuyển phát như địa chỉ để họ có thể thực hiện hành động. Bạn cũng có thể giới hạn hộp thư theo dõi để chỉ bắt đầu trước đây là địa chỉ email hợp lệ. 

Bất kỳ hộp thư nào nắm bắt tất cả sẽ nhận được nhiều thư rác và cuối cùng có thể điền vào nếu không được giám sát chặt chẽ. (Có các giới hạn tiếp nhận.) 

Nếu bạn quyết định tiếp tục, hãy làm theo các bước sau đây:

1. Tạo một nhóm phân phối động & bao gồm "tất cả các loại người nhận."

2. Tạo hộp thư chuyên biệt để bắt email, ví dụ, catchall@domain.com.

3. Đối với tên miền cụ thể, hãy đặt kiểu DomainType thành "InternalRelay". Nếu sau đó bạn loại bỏ tất cả bắt kịp, hãy đảm bảo đặt tên miền trở lại thẩm quyền.

4. Tạo một quy tắc truyền dẫn dòng thư như sau:

    - Nếu người gửi là "bên ngoài tổ chức"
    - Chuyển hướng thư đến Catchall@domain.com
    - Trừ khi người nhận là thành viên của allusers@domain.com (nhóm phân phối chứa tất cả thành viên)
    - Đảm bảo xác thực rằng các hộp thư mới được thêm vào nhóm phân phối động
