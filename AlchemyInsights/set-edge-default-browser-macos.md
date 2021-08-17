---
title: Đặt Microsoft Edge làm trình duyệt mặc định trên thiết bị macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: e04f8931ef12c426a5c3d5f617fc5f5d5c3a15c6fe43f7b84a7e97e8ee04e3fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54073982"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>Đặt Microsoft Edge làm trình duyệt mặc định trên thiết bị macOS

Sử dụng một trong hai phương pháp sau đây để Microsoft Edge đặt làm trình duyệt mặc định:

Phương pháp 1: Làm cho thiết bị có hình ảnh macOS Microsoft Edge đã được đặt làm trình duyệt mặc định.

Phương pháp 2: Đặt chính sách DefaultBrowserSettingEnabled để nhắc người dùng đặt cài Microsoft Edge đặt làm trình duyệt mặc định.

Phương pháp này cho phép người dùng thay đổi trình duyệt mặc định. Vì lý do này, chúng tôi khuyên bạn nên triển khai chính sách DefaultBrowserSettingEnabled ngay cả khi bạn đã sử dụng phương pháp 1. Nếu người dùng thay đổi trình duyệt mặc định sau khi chính sách được triển khai, chính sách sẽ nhắc người dùng đặt trình duyệt mặc định trở về chế Microsoft Edge.
