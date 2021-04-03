---
title: Khóa phục hồi BitLocker
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
- "1922"
- "9000220"
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505090"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Truy nhập khóa phục hồi BitLocker

Khi cấu hình thiết đặt BitLocker InTune Endpoint Protection Policy, có thể xác định việc lưu trữ thông tin phục hồi BitLocker trong Azure Active Directory hay không.

Nếu cài đặt đó được cấu hình, dữ liệu phục hồi được lưu trữ sẽ được hiển thị với một người quản trị InTune như là một phần của dữ liệu bản ghi thiết bị trong lưỡi trong thiết bị InTune theo hai cách:

Thiết bị-Azure AD Devices-> "thiết bị" hoặc thiết bị-> tất cả các thiết bị-> "thiết bị"-các khóa phục hồi >

Ngoài ra, nếu có quyền truy nhập quản trị cho chính thiết bị, khóa khôi phục (mật khẩu), bạn có thể nhìn thấy lệnh này bằng cách chạy lệnh sau đây từ dấu nhắc lệnh nâng cao:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Nếu thiết bị đã được mã hóa trước khi đăng ký trong InTune, khóa khôi phục có thể đã được liên kết với "tài khoản Microsoft" (MSA) được sử dụng để đăng nhập vào thiết bị trong quá trình OOBE. Nếu đó là trường hợp, hãy truy cập  https://onedrive.live.com/recoverykey và đăng nhập bằng MSA nên hiển thị các thiết bị mà các khóa phục hồi được lưu trữ.
 
Nếu thiết bị đã được mã hóa là kết quả của việc cấu hình thông qua chính sách nhóm dựa trên tên miền, thông tin phục hồi có thể được lưu trữ trong Active Directory tại chỗ.

Nếu bạn đã cấu hình chính sách bảo vệ Endpoint để lưu trữ khóa phục hồi trong Azure Active Directory nhưng khóa cho một thiết bị cụ thể chưa được tải lên, bạn có thể kích hoạt tải lên bằng cách xoay khóa phục hồi cho thiết bị đó từ bảng điều khiển MEM. Để biết chi tiết, hãy xem [xoay phím phục hồi BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

