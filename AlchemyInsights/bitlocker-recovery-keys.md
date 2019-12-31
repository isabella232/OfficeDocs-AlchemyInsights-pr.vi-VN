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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="873f4-102">Truy cập khóa phục hồi BitLocker</span><span class="sxs-lookup"><span data-stu-id="873f4-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="873f4-103">Khi cấu hình cài đặt BitLocker InTune Endpoint Protection chính sách, có thể xác định xem BitLocker phục hồi thông tin sẽ được lưu trữ trong Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="873f4-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="873f4-104">Nếu cài đặt đó được cấu hình, dữ liệu khôi phục được lưu trữ sẽ hiển thị cho quản trị viên InTune là một phần của dữ liệu bản ghi thiết bị trong bộ phận thiết bị máy cắt theo hai cách:</span><span class="sxs-lookup"><span data-stu-id="873f4-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="873f4-105">Thiết bị-thiết bị Azure AD-> "thiết bị" hoặc thiết bị-> tất cả thiết bị-> "thiết bị"-> phím khôi phục</span><span class="sxs-lookup"><span data-stu-id="873f4-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="873f4-106">Ngoài ra, nếu có quyền truy cập quản trị vào thiết bị, khóa khôi phục (mật khẩu) có thể được nhìn thấy bằng cách chạy lệnh sau từ dấu nhắc lệnh nâng cao:</span><span class="sxs-lookup"><span data-stu-id="873f4-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="873f4-107">Nếu thiết bị được mã hoá trước khi đăng ký InTune, khôi phục khoá có thể đã được liên kết với "Microsoft Account" (MSA) được sử dụng để đăng nhập vào thiết bị trong quá trình OOBE.</span><span class="sxs-lookup"><span data-stu-id="873f4-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="873f4-108">Nếu đó là trường hợp, truy https://onedrive.live.com/recoverykey cập và đăng nhập với MSA nên hiển thị các thiết bị mà khóa khôi phục được lưu trữ.</span><span class="sxs-lookup"><span data-stu-id="873f4-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="873f4-109">Nếu thiết bị được mã hóa là kết quả của cấu hình thông qua chính sách nhóm dựa trên miền, thông tin khôi phục có thể được lưu trữ trong Active Directory tại nơi.</span><span class="sxs-lookup"><span data-stu-id="873f4-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

