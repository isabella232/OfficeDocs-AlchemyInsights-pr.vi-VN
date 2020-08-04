---
title: Tự động dọn dẹp các thiết bị cũ trong InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555739"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Tự động dọn dẹp các thiết bị cũ trong InTune

InTune cho phép quản trị viên để cấu hình một khoảng thời gian giữa 90 và 270 ngày, sau đó các thiết bị cũ được loại bỏ khỏi Dịch vụ. Thiết lập này là tổ chức rộng và một khi kích hoạt đi vào hiệu lực ngay lập tức. Bất kỳ thiết bị nào không được kiểm tra vào máy chủ InTune trong một khoảng thời gian vượt quá cài đặt sẽ bị xóa vĩnh viễn.

**Lưu ý** Chỉ MDM thiết bị đối tượng đủ điều kiện cho hành động dọn dẹp này. EAS chỉ đối tượng thiết bị được loại trừ.

Để biết thêm thông tin về khi thiết bị đủ điều kiện để xóa dựa trên cài đặt thiết bị dọn dẹp và "trạng thái":

Cài đặt: **xóa thiết bị sau ngày Check-in cuối cùng: có (một số giá trị (N) trong ngày đã chỉ định)**

- Dựa trên giá trị (N) được cấu hình trong cài đặt, Dịch vụ InTune xoá thiết bị trong những ngày được chỉ định sau khi nó cuối cùng kiểm tra thành công.

Cài đặt: **xóa thiết bị sau ngày nhận phòng cuối cùng: không**

- 180 ngày sau khi chứng chỉ thiết bị hết hạn và không được gia hạn, thiết bị sẽ bị xóa.

**Lưu ý** Trong cả hai trường hợp, thiết bị phải được đăng ký thành công trong InTune. Đăng ký xảy ra trong thiết bị đầu tiên checkin với dịch vụ InTune.

Nếu thiết bị ghi thành công để InTune nhưng không trở thành InTune đăng ký, thiết bị sẽ bị xóa 270 ngày sau khi đăng ký. (90 ngày để đánh dấu thiết bị như thu hồi, và sau đó một 180 ngày để xóa hồ sơ.)

Không có cơ chế nào tồn tại trong bảng điều khiển InTune để thiết lập ngày hết hạn của chứng nhận thiết bị cho bất kỳ thiết bị nào.