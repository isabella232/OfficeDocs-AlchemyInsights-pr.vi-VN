---
title: Lỗi đồng bộ hóa đăng ký thiết bị tự động của Apple
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
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448944"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Lỗi đồng bộ hóa đăng ký thiết bị tự động của Apple

"Chúng tôi đã phát hiện rằng bạn có một hoặc nhiều thẻ ADE/DEP nằm trong trạng thái lỗi. Cho đến khi trạng thái lỗi được giải quyết cho từng mã thông báo bị ảnh hưởng, chức năng ADE sẽ không hoạt động như mong đợi. ".

Lỗi này có thể hiển thị trong một số cách bao gồm:

1. Các thiết bị có thể không đồng bộ từ ABM/ASM vào InTune
2. Các bài tập hồ sơ đăng ký có thể không
3. Thiết bị có thể không hoàn tất việc đăng ký ADE thành công

Kiểm tra lỗi đồng bộ được báo cáo trong bảng điều khiển InTune bên dưới **thiết bị > đăng ký thiết bị > các thẻ chương trình đăng ký > của Apple**.

Một trong những nguyên nhân phổ biến nhất của lỗi đồng bộ là hết hạn của mã thông báo hiện tại. Trong nhiều trường hợp, việc gia hạn mã thông báo bị ảnh hưởng sẽ giải quyết được sự cố.

Nếu một hoặc nhiều thẻ của bạn đã hết hạn, hãy xem tài liệu sau đây để giúp bạn gia hạn chúng là phù hợp:

[Gia hạn mã thông báo đăng ký thiết bị tự động](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Ngoài ra, bạn có thể thấy các tài liệu sau đây để xem những điều chỉnh sửa tiềm ẩn cho các lỗi khác khiến đồng bộ hóa mã lỗi:

[Lỗi đồng bộ ABM/ASM cho iOS/iPadOS và thẻ đăng ký thiết bị tự động macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Lỗi đồng bộ ABM/ASM cho iOS/iPadOS và thẻ đăng ký thiết bị tự động macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
