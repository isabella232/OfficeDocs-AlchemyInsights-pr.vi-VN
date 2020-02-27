---
title: Tạo một email bắt tất cả
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286313"
---
# <a name="create-an-email-catch-all"></a>Tạo một email bắt tất cả

Sử dụng một nắm bắt tất cả được khuyến khích mạnh mẽ. Nó là tốt hơn để cung cấp một thư bị trả lại cho người gửi cho phép gửi biết tin nhắn của họ không thể được gửi như là địa chỉ để họ có thể thực hiện hành động. Bạn cũng có thể hạn chế hộp thư theo dõi để chỉ bắt trước đây địa chỉ email hợp lệ. 

Bất kỳ bắt tất cả các hộp thư sẽ nhận được một thỏa thuận tốt của thư rác và cuối cùng có thể điền nếu không theo dõi chặt chẽ. (Có những giới hạn nhận được.) 

Nếu bạn quyết định tiếp tục, hãy làm theo các bước sau:

1. Tạo nhóm phân phối động & bao gồm "tất cả các loại người nhận."

2. Tạo một hộp thư chuyên dụng để bắt email, ví dụ: catchall@domain.com.

3. Đối với miền cụ thể, đặt DomainType "InternalRelay". Nếu sau đó bạn loại bỏ tất cả các bắt, hãy chắc chắn để đặt tên miền trở lại uỷ quyền.

4. Tạo quy tắc truyền tải Mailflow như sau:

    - Nếu người gửi là "bên ngoài tổ chức"
    - Chuyển hướng thư đến Catchall@domain.com
    - Ngoại trừ nếu người nhận là thành viên của allusers@domain.com (nhóm phân phối chứa tất cả các thành viên)
    - Đảm bảo xác nhận rằng hộp thư mới được thêm vào nhóm phân phối động
