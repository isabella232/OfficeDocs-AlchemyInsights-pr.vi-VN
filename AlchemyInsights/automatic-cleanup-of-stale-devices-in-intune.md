---
title: Tự động dọn dẹp các thiết bị cũ trong InTune
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
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715043"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Tự động dọn dẹp các thiết bị cũ trong InTune

InTune cho phép người quản trị cấu hình khoảng thời gian giữa 90 và 270 ngày, sau khi các thiết bị cũ được loại bỏ khỏi Dịch vụ. Thiết đặt này là tổ chức rộng và đã kích hoạt một lần sẽ có hiệu lực ngay lập tức. Mọi thiết bị không được kiểm nhập vào máy chủ InTune trong một khoảng thời gian vượt quá thiết đặt sẽ bị xóa vĩnh viễn.

**Ghi chú** Chỉ các đối tượng thiết bị MDM đủ điều kiện cho hành động dọn dẹp này. Chỉ các đối tượng của thiết bị EAS được loại trừ.

Để biết thêm thông tin về khi thiết bị trở nên đủ điều kiện để xóa căn cứ theo thiết đặt thiết bị dọn dẹp và trạng thái "của bạn":

Thiết đặt: **xóa các thiết bị sau ngày kiểm nhập lần cuối: có (một số giá trị (N) trong các ngày đã xác định)**

- Dựa trên giá trị (N) được đặt cấu hình trong thiết đặt, Dịch vụ InTune sẽ xóa thiết bị trong những ngày cụ thể sau khi kiểm tra thành công lần cuối.

Thiết đặt:  **xóa các thiết bị sau ngày kiểm nhập lần cuối: không có**

- 180 ngày sau khi chứng chỉ thiết bị hết hạn và không được gia hạn, thiết bị sẽ bị xóa.

**Ghi chú** Trong cả hai trường hợp, thiết bị phải được đăng ký thành công trong InTune. Đăng ký xảy ra trong trình kiểm tra thiết bị đầu tiên với dịch vụ InTune.

Nếu thiết bị đã được thực hiện thành công với InTune nhưng không trở thành InTune đã đăng ký, thiết bị sẽ bị xóa 270 ngày sau khi ghi danh. (90 ngày để đánh dấu thiết bị là thu hồi, rồi sau đó 180 ngày khác để xóa bản ghi.)

Không có cơ chế hiện tại trong giao diện điều khiển InTune để thiết lập ngày hết hạn của chứng chỉ thiết bị cho bất kỳ thiết bị nào đã cho.