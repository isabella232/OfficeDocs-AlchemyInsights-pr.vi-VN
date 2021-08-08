---
title: Khóa khôi phục Bitlocker
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
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060086"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Truy nhập khóa khôi phục Bitlocker

Khi đặt cấu hình cài đặt Bitlocker Chính sách Bảo vệ Điểm cuối Intune, bạn có thể xác định xem thông tin phục hồi Bitlocker có được lưu trữ trong Azure Active Directory.

Nếu cài đặt đó được đặt cấu hình thì người quản trị Intune sẽ hiển thị dữ liệu phục hồi được lưu trữ dưới dạng một phần của dữ liệu bản ghi thiết bị trong Intune Devices bằng hai cách:

Thiết bị - Thiết bị Azure AD -> "Thiết bị" OR Thiết bị -> Tất cả Thiết bị -> 2 "Thiết bị" -Khóa khôi > hồi

Ngoài ra, nếu có quyền truy nhập quản trị vào chính thiết bị đó, bạn có thể xem khóa khôi phục (Mật khẩu) bằng cách chạy lệnh sau đây từ lời nhắc chỉ lệnh mức cao:

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
Nếu thiết bị đã được mã hóa trước khi đăng ký trong Intune, khóa khôi phục có thể đã được liên kết với "Tài khoản Microsoft" (MSA) được sử dụng để đăng nhập vào thiết bị trong quy trình OOBE. Nếu đúng như vậy, việc truy nhập và đăng nhập bằng MSA đó sẽ hiển thị các thiết bị mà khóa khôi  https://onedrive.live.com/recoverykey phục đã được lưu trữ.
 
Nếu thiết bị đã được mã hóa do cấu hình thông qua chính sách nhóm dựa trên miền, thông tin phục hồi có thể được lưu trữ trong Active Directory tại chỗ.

Nếu bạn đã đặt cấu hình Chính sách bảo vệ điểm cuối để lưu trữ khóa khôi phục trong Azure Active Directory nhưng khóa cho một thiết bị cụ thể chưa được tải lên, bạn có thể kích hoạt quá trình tải lên bằng cách xoay khóa khôi phục cho thiết bị đó từ bảng điều khiển MEM. Để biết chi tiết, [hãy xem Xoay khóa khôi phục BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

