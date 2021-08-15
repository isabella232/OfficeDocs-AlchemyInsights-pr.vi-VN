---
title: Lỗi đồng bộ Đăng ký Thiết bị Tự động của Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013770"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Lỗi đồng bộ Đăng ký Thiết bị Tự động của Apple

"Chúng tôi đã phát hiện rằng bạn có một hoặc nhiều Mã thông báo ADE/DEP đang ở trạng thái lỗi. Cho đến khi trạng thái lỗi được giải quyết cho mỗi mã thông báo bị ảnh hưởng, chức năng ADE sẽ không hoạt động như mong đợi.".

Lỗi này có thể xuất hiện theo một số cách, bao gồm:

1. Thiết bị có thể không đồng bộ hóa từ ABM/ASM sang Intune
2. Việc gán hồ sơ đăng ký có thể không thành công
3. Thiết bị có thể không hoàn thành đăng ký ADE thành công

Kiểm tra lỗi đồng bộ được báo cáo trong bảng điều khiển Intune bên dưới thiết bị > Đăng ký thiết > đăng ký Apple > mã thông báo chương **trình Đăng ký**.

Một trong những nguyên nhân phổ biến nhất của lỗi đồng bộ là hết hạn mã thông báo hiện tại. Trong nhiều trường hợp, việc gia hạn mã thông báo bị ảnh hưởng sẽ giải quyết được sự cố.

Nếu một hoặc nhiều mã thông báo của bạn đã hết hạn, hãy xem tài liệu sau đây để giúp bạn gia hạn mã cho phù hợp:

[Gia hạn mã thông báo Đăng ký Thiết bị Tự động](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Ngoài ra, bạn có thể xem tài liệu sau đây để xem các phương pháp khắc phục tiềm tàng cho lỗi khác gây ra lỗi đồng bộ hóa mã thông báo:

[Lỗi Đồng bộ ABM/ASM cho iOS/iPadOS và mã thông báo Đăng ký Thiết bị Tự động macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Lỗi Đồng bộ ABM/ASM cho iOS/iPadOS và mã thông báo Đăng ký Thiết bị Tự động macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
