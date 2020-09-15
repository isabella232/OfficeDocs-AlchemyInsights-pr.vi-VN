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
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685908"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="47705-102">Truy nhập khóa phục hồi BitLocker</span><span class="sxs-lookup"><span data-stu-id="47705-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="47705-103">Khi cấu hình thiết đặt BitLocker InTune Endpoint Protection Policy, có thể xác định việc lưu trữ thông tin phục hồi BitLocker trong Azure Active Directory hay không.</span><span class="sxs-lookup"><span data-stu-id="47705-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="47705-104">Nếu cài đặt đó được cấu hình, dữ liệu phục hồi được lưu trữ sẽ được hiển thị với một người quản trị InTune như là một phần của dữ liệu bản ghi thiết bị trong lưỡi trong thiết bị InTune theo hai cách:</span><span class="sxs-lookup"><span data-stu-id="47705-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="47705-105">Thiết bị-Azure AD Devices-> "thiết bị" hoặc thiết bị-> tất cả các thiết bị-> "thiết bị"-các khóa phục hồi ></span><span class="sxs-lookup"><span data-stu-id="47705-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="47705-106">Ngoài ra, nếu có quyền truy nhập quản trị cho chính thiết bị, khóa khôi phục (mật khẩu), bạn có thể nhìn thấy lệnh này bằng cách chạy lệnh sau đây từ dấu nhắc lệnh nâng cao:</span><span class="sxs-lookup"><span data-stu-id="47705-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="47705-107">Nếu thiết bị đã được mã hóa trước khi đăng ký trong InTune, khóa khôi phục có thể đã được liên kết với "tài khoản Microsoft" (MSA) được sử dụng để đăng nhập vào thiết bị trong quá trình OOBE.</span><span class="sxs-lookup"><span data-stu-id="47705-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="47705-108">Nếu đó là trường hợp, hãy truy cập  https://onedrive.live.com/recoverykey và đăng nhập bằng MSA nên hiển thị các thiết bị mà các khóa phục hồi được lưu trữ.</span><span class="sxs-lookup"><span data-stu-id="47705-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="47705-109">Nếu thiết bị đã được mã hóa là kết quả của việc cấu hình thông qua chính sách nhóm dựa trên tên miền, thông tin phục hồi có thể được lưu trữ trong Active Directory tại chỗ.</span><span class="sxs-lookup"><span data-stu-id="47705-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

