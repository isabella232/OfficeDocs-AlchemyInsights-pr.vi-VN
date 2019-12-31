---
title: Khóa phục hồi BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908836"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Truy cập khóa phục hồi BitLocker

Khi cấu hình cài đặt BitLocker InTune Endpoint Protection chính sách, có thể xác định xem BitLocker phục hồi thông tin sẽ được lưu trữ trong Azure Active Directory.

Nếu cài đặt đó được cấu hình, dữ liệu khôi phục được lưu trữ sẽ hiển thị cho quản trị viên InTune là một phần của dữ liệu bản ghi thiết bị trong bộ phận thiết bị máy cắt theo hai cách:

Thiết bị-thiết bị Azure AD-> "thiết bị" hoặc thiết bị-> tất cả thiết bị-> "thiết bị"-> phím khôi phục

Ngoài ra, nếu có quyền truy cập quản trị vào thiết bị, khóa khôi phục (mật khẩu) có thể được nhìn thấy bằng cách chạy lệnh sau từ dấu nhắc lệnh nâng cao:

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
Nếu thiết bị được mã hoá trước khi đăng ký InTune, khôi phục khoá có thể đã được liên kết với "Microsoft Account" (MSA) được sử dụng để đăng nhập vào thiết bị trong quá trình OOBE. Nếu đó là trường hợp, truy https://onedrive.live.com/recoverykey cập và đăng nhập với MSA nên hiển thị các thiết bị mà khóa khôi phục được lưu trữ.
 
Nếu thiết bị được mã hóa là kết quả của cấu hình thông qua chính sách nhóm dựa trên miền, thông tin khôi phục có thể được lưu trữ trong Active Directory tại nơi.
 

