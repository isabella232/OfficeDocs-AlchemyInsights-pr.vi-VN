---
title: 1065 lưu lại địa chỉ IP của EOP Outbound rangesMC146155
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
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806817"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Deprecation của dải địa chỉ IP đi đến EOP

Chúng tôi đã phát hiện ra một vấn đề tiềm ẩn với tổ chức của bạn (nếu không được sửa vào ngày 26 tháng 10, 2018) có thể ngắt dòng thư đến đích tại chỗ hoặc bên ngoài của bạn. Như truyền đạt được trước đó, để đơn giản hóa việc quản lý dải địa chỉ IP, chúng tôi đang củng cố phạm vi địa chỉ IP của Exchange Online Protection (EOP) được dùng để gửi và nhận email bên ngoài Microsoft 365. Phân tích của chúng tôi cho biết một hoặc nhiều nguồn email bên ngoài hoặc các đích mà bạn đã cấu hình trong các đường kết nối dòng thư không chấp nhận kết nối từ dải địa chỉ IP được hiển thị [ở đây](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Act trước ngày 26 tháng 10 để đảm bảo các nguồn và đích này sẽ chấp nhận kết nối đến và từ tất cả các [địa chỉ IP đã phát hành của EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Để biết thêm thông tin về thay đổi này, vui lòng xem Trung tâm thông báo bài viết [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)hoặc [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Lưu ý**: nếu trước đó bạn đã sử dụng IP hoặc URL phát hành qua HTML, XML và RSS cho các bản Cập Nhật điểm cuối, bạn cũng nên di chuyển đến các dịch vụ web mới để tự động hóa các kiểu bản cập nhật này. Để biết thêm thông tin, hãy xem [thể loại điểm cuối microsoft 365 và địa chỉ IP của microsoft 365 và dịch vụ web URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
