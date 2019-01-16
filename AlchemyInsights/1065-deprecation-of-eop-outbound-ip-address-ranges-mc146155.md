---
title: 1065 deprecation EOP outbound IP địa chỉ rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28320488"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Deprecation EOP ra ngoài phạm vi địa chỉ IP

Chúng tôi đã phát hiện một vấn đề tiềm năng với các tổ chức của bạn (nếu không được sửa chữa bởi 26 tháng 10 năm 2018) có thể phá vỡ luồng thư đến chỗ hoặc bên ngoài các điểm đến của bạn. Như là trước đó đã truyền đạt, để đơn giản hóa quản lý phạm vi địa chỉ IP, chúng tôi đang củng cố các dải địa chỉ IP bảo vệ trực tuyến trao đổi (EOP), được sử dụng để gửi và nhận thư điện tử bên ngoài của Office 365. Phân tích của chúng tôi cho thấy rằng một hoặc nhiều e-mail bên ngoài nguồn hoặc điểm đến mà bạn đã đặt cấu hình trong thư lưu lượng kết nối không chấp nhận kết nối từ IP địa chỉ phạm vi Hiển thị [ở đây](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Hoạt động trước ngày 26 tháng 10 để đảm bảo các nguồn và các điểm đến sẽ chấp nhận kết nối đến và đi từ tất cả [xuất bản EOP IP địa chỉ](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Để biết thêm chi tiết về sự thay đổi này, hãy xem Trung tâm thông báo bài viết [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)hoặc [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).
  
 **Lưu ý**: nếu trước đây bạn sử dụng IP hoặc URL xuất bản thông qua HTML, XML, và RSS endpoint Cập Nhật, bạn cũng nên di chuyển sử dụng các dịch vụ web mới cho các loại bản cập nhật tự động. Để biết thêm chi tiết, hãy xem [Office 365 endpoint thể loại và Office 365 địa chỉ IP và URL trang web dịch vụ](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
  

