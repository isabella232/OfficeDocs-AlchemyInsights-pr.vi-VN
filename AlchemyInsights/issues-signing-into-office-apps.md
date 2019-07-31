---
title: Vấn đề đăng nhập vào ứng dụng văn phòng
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938392"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Sửa chữa thông báo "máy tính của bạn tin cậy nền tảng mô-đun không hoạt động đúng" ứng dụng văn phòng

Để khắc phục lỗi này, hãy thử như sau:

- Cài đặt các bản cập nhật mới nhất cho [Windows](https://support.microsoft.com/help/4027667/windows-10-update) và [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Rõ ràng văn phòng thông tin đăng nhập](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) bằng cách sử dụng trình quản lý ủy nhiệm của Windows.<br/>
    **Lưu ý:** Các đường dẫn đăng ký đối với Office 2016 đã thay đổi để 16.0. (Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)
- Hãy thử [sử dụng quá trình phục hồi](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) sửa chữa Trusted Platform Module (TPM) thất bại.
- Thiết lập EnableADAL = 0, bằng cách sử dụng các bước sau:  
    1. Nhấp chuột phải vào nút Start của Windows, chọn **Run**, gõ **regedit**, và sau đó chọn **OK**.
    2. Chọn **có** để cho phép trình biên tập Registry để thay đổi thiết bị của bạn.
    3. Trong Registry Editor, thêm một giá trị DWORD của **EnableADAL** với một thiết lập **0** theo HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Để biết thêm chi tiết, hãy xem [kết nối các vấn đề trong đăng nhập sau khi Cập Nhật cho Office 2016 build 16.0.7967 trên Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).