---
title: 1065 Việc bỏ dùng Dải địa chỉ IP đi EOPMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031284"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Bỏ dùng Dải địa chỉ IP đi EOP

Chúng tôi đã phát hiện một sự cố tiềm tàng với tổ chức của bạn mà (nếu không được sửa trước 26/10/2018) có thể làm ngắt dòng thư đến đích tại chỗ hoặc đích bên ngoài của bạn. Như đã truyền đạt trước đây, để đơn giản hóa việc quản lý dải địa chỉ IP, chúng tôi đang hợp nhất dải địa chỉ IP Exchange Online Protection (EOP) được dùng để gửi và nhận email bên ngoài Microsoft 365. Phân tích của chúng tôi cho biết rằng một hoặc nhiều nguồn email hoặc đích bên ngoài mà bạn đã đặt cấu hình trong bộ nối dòng thư không chấp nhận kết nối từ dải địa chỉ IP được hiển thị [ở đây.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Hành động trước 26 Tháng Mười để đảm bảo các nguồn và đích này sẽ chấp nhận các kết nối đến và từ tất cả các [địa chỉ IP EOP đã phát hành.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Để biết thêm thông tin về thay đổi này, vui lòng xem bài đăng trong Trung tâm Thông báo [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)hoặc [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Lưu** ý: Nếu trước đây bạn đã sử dụng IP hoặc URL phát hành qua HTML, XML và RSS để cập nhật điểm cuối, bạn cũng nên di chuyển sang các dịch vụ web mới để tự động hóa các loại cập nhật này. Để biết thêm thông tin, hãy [xem Microsoft 365 danh mục điểm cuối và Microsoft 365 địa chỉ IP và dịch vụ web URL mới.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
