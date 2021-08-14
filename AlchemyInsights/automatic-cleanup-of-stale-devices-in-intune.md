---
title: Tự động dọn dẹp thiết bị cũ trong Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 905881f08ace7afae871ac48fa30ed1a0f15d13972cdff299a6694ca2eafc9cc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53997114"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Tự động dọn dẹp thiết bị cũ trong Intune

Intune cho phép người quản trị đặt cấu hình khoảng thời gian từ 90 đến 270 ngày, sau đó các thiết bị cũ sẽ được loại bỏ khỏi dịch vụ. Cài đặt này có phạm vi toàn tổ chức và sau khi kích hoạt sẽ có hiệu lực ngay lập tức. Bất kỳ thiết bị nào không được kiểm nhập vào máy chủ Intune trong một khoảng thời gian vượt quá thiết đặt sẽ bị xóa vĩnh viễn.

**Lưu ý** Chỉ các đối tượng của thiết bị MDM đủ điều kiện cho hành động dọn sạch này. Chỉ loại trừ các đối tượng của thiết bị EAS.

Để biết thêm thông tin về thời điểm thiết bị đủ điều kiện để xóa dựa trên thiết đặt dọn sạch thiết bị và "trạng thái" của thiết bị:

Cài đặt: **Xóa thiết bị sau ngày kiểm nhập gần nhất: Có (một số giá trị (N) trong ngày đã xác định)**

- Dựa trên giá trị (N) được đặt cấu hình trong cài đặt, dịch vụ Intune sẽ xóa thiết bị trong những ngày được chỉ định sau lần kiểm nhập thành công gần nhất.

Cài đặt:  **Xóa thiết bị sau ngày kiểm nhập gần nhất: Không**

- 180 ngày sau khi chứng chỉ thiết bị hết hạn và không được gia hạn, thiết bị sẽ bị xóa.

**Lưu ý** Trong cả hai trường hợp, thiết bị phải được đăng ký thành công trong Intune. Việc đăng ký diễn ra trong quá trình kiểm tra thiết bị đầu tiên với dịch vụ Intune.

Nếu một thiết bị đăng ký thành công Intune nhưng không trở thành đã đăng ký Intune, thiết bị sẽ bị xóa sau 270 ngày đăng ký. (90 ngày để đánh dấu thiết bị là đã thu hồi, rồi thêm 180 ngày nữa để xóa bản ghi.)

Hiện tại không có cơ chế nào trong bảng điều khiển Intune để thiết lập ngày hết hạn của chứng nhận thiết bị cho mọi thiết bị nhất định.