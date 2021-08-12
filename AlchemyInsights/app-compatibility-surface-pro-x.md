---
title: Tính tương thích của ứng dụng với Microsoft Surface Pro X
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7009"
- "9003951"
ms.openlocfilehash: 8f353d1337415183db1df168406b33594fb5fdb0aac3f13d0afe3e682fa6e3f3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932047"
---
# <a name="app-compatibility-with-microsoft-surface-pro-x"></a>Tính tương thích của ứng dụng với Microsoft Surface Pro X

Các ứng dụng chạy khác nhau trên các thiết bị Surface Pro X. Hầu hết các ứng dụng đều tương thích, tuy nhiên, có một số hạn chế. Đây là danh sách các sự cố bạn có thể gặp phải trong khi chạy ứng dụng: 

**Trình điều khiển.** Trình điều khiển sẽ hoạt động nếu được thiết kế dành cho Windows 10 PC hoạt động trên nền ARM. Nếu trình điều khiển không hoạt động, thì ứng dụng—hoặc phần cứng mà nó dựa vào—cũng sẽ không hoạt động. Để được hỗ trợ thêm với thiết bị của bạn, [hãy xem Windows 10 hỏi](https://support.microsoft.com/windows/windows-10-arm-based-pcs-faq-477f51df-2e3b-f68f-31b0-06f5e4f8ebb5) thường gặp về PC dựa trên ARM hoặc hỏi nhà sản xuất phần cứng.

**Ứng dụng 64 bit (x64).** Các ứng dụng 64 bit (x64) sẽ không hoạt động. Bạn sẽ cần các ứng dụng 64 bit (ARM64), ứng dụng 32 bit (ARM32) hoặc ứng dụng 32 bit (x86). Thông thường, bạn có thể tìm thấy các phiên bản ứng dụng 32 bit (x86) nhưng một số nhà phát triển ứng dụng chỉ cung cấp các ứng dụng 64 bit (x64).

**Ứng dụng được tùy chỉnh.** Các ứng dụng tùy chỉnh trải Windows năng, như công nghệ hỗ trợ hay ứng dụng lưu trữ đám mây, có thể gặp sự cố. Để tìm hiểu thêm, hãy hỏi nhà sản xuất ứng dụng.

**Phần mềm chống vi-rút của bên thứ ba.** Không cài đặt được một số phần mềm chống vi-rút của bên thứ ba. Bảo mật Windows giúp giữ an toàn cho bạn trong thời hạn được hỗ trợ trên thiết bị của Windows 10 bạn.

**Windows Fax và Quét.** Ứng Windows Fax và Quét không khả dụng trên PC Windows 10 nền ARM.

Nếu bạn thấy mình gặp sự cố khi cài đặt, gỡ cài đặt hoặc cài đặt lại ứng dụng, hãy xem Chi tiết khắc [phục sự cố ứng dụng](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-app-install#app-troubleshooting-details).

Ngoại trừ trong trường hợp hiếm gặp, tất cả các từ khóa phải là OR chứ không phải AND.