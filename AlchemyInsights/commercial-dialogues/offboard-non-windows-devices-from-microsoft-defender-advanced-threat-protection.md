---
title: Bảo vệ khỏi mối đe dọa Windows từ Tính năng Chống Mối đe dọa Nâng cao của Bộ bảo vệ Microsoft (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fbaab348e06691b73db68492a0083c4a5a54c4504e03d27ec53f2a9f5047266d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967823"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Bảo vệ khỏi mối đe dọa Windows từ Tính năng Chống Mối đe dọa Nâng cao của Bộ bảo vệ Microsoft (ATP)

Dưới đây là cách thực hiện:

1. Làm theo hướng dẫn sử dụng của bên thứ ba để ngắt kết nối giải pháp của bên thứ ba khỏi ATP của Bộ bảo vệ Microsoft.
2. Từ đối tượng Azure Active Directory của bạn, hãy loại bỏ các quyền cho giải pháp của bên thứ ba:

    1. Đăng nhập vào cổng [thông tin Azure](https://go.microsoft.com/fwlink/?linkid=2125612).
    1. Chọn **Tất cả dịch** vụ  >  **Azure Active Directory** Enterprise  >  **Applications**.
    1. Chọn ứng dụng bạn muốn bỏ qua.
    1. Chọn **Xóa**.

Để tìm hiểu thêm, hãy [xem mục Các thiết bị không sử dụng bàn Windows của bạn.](https://go.microsoft.com/fwlink/?linkid=2143630)
