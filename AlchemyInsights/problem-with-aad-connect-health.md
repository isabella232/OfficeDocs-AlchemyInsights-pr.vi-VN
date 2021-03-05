---
title: Vấn đề với thiết bị cảm ứng của Bad Connect
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483125"
---
# <a name="problem-with-aad-connect-health"></a>Vấn đề với thiết bị cảm ứng của Bad Connect

- Đảm bảo rằng bạn được phép thực hiện thao tác này. Người quản trị toàn cầu có quyền truy nhập theo mặc định. Ngoài ra, bạn có thể sử dụng [điều khiển truy nhập dựa trên vai trò](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) để cho phép người đóng góp đăng ký.
- Đảm bảo các điểm cuối bắt buộc được kích hoạt và không bị chặn do tường lửa. Để biết chi tiết, hãy xem mục [yêu cầu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Đăng ký có thể không thành công vì giao tiếp đi là phải chịu việc kiểm tra SSL bằng tầng mạng.
- Đảm bảo rằng bạn đã xác minh cài đặt thông báo cho Azure AD Connect Health. Vui lòng xem lại thiết đặt của bạn. [Hướng dẫn](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) này có thể giúp bạn hiểu cách cấu hình các thiết đặt thông báo cho Azure AD Connect Health Notifications.
- Để tìm hiểu thêm về báo cáo đồng bộ hóa trạng thái kết nối và cách tải xuống, hãy xem [báo cáo đồng bộ hóa mức đối tượng](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Để khắc phục sự cố về cảnh báo trạng thái kết nối, hãy làm theo [các hướng dẫn khắc phục sự cố cho các cảnh báo tự động kết nối dữ liệu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) và cho các câu hỏi thường gặp, hãy xem các [câu hỏi cài đặt kết nối thông thường](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)của cộng đồng.
