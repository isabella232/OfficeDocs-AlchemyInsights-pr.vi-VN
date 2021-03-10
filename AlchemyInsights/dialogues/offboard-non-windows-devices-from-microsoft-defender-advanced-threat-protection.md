---
title: Các thiết bị không phải Windows không có từ bộ bảo vệ mối đe dọa nâng cao của Microsoft Defender (ATP)
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695165"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Các thiết bị không phải Windows không có từ bộ bảo vệ mối đe dọa nâng cao của Microsoft Defender (ATP)

Dưới đây là cách thực hiện:

1. Hãy làm theo các tài liệu hướng dẫn bên thứ ba để ngắt kết nối giải pháp bên thứ ba từ Microsoft Defender ATP.
2. Từ đối tượng thuê Azure Active Directory của bạn, hãy loại bỏ quyền cho giải pháp của bên thứ ba:

    1. Đăng nhập vào [cổng thông tin Azure](https://go.microsoft.com/fwlink/?linkid=2125612).
    1. Chọn **tất cả**  >  các ứng dụng dịch vụ **Azure Active Directory**  >  **Enterprise**.
    1. Chọn ứng dụng bạn muốn offboard.
    1. Chọn **xóa**.

Để tìm hiểu thêm, hãy xem các [thiết bị không](https://go.microsoft.com/fwlink/?linkid=2143630)phải của Windows.
