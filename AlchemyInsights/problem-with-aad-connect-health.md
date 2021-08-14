---
title: Sự cố với Trạng Kết nối AAD
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
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923774"
---
# <a name="problem-with-aad-connect-health"></a>Sự cố với Trạng Kết nối AAD

- Đảm bảo bạn được phép thực hiện thao tác. Người quản trị toàn cục có quyền truy nhập theo mặc định. Ngoài ra, bạn có thể sử dụng [Kiểm soát Truy nhập Dựa trên Vai trò đối](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) với quyền đăng ký đại diện cho Người đóng góp.
- Đảm bảo các điểm cuối bắt buộc được bật và không bị chặn do tường lửa. Để biết chi tiết, hãy xem [yêu cầu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Việc đăng ký có thể không thành công do giao tiếp đi phải được kiểm tra SSL bởi tầng mạng.
- Đảm bảo rằng bạn đã xác minh cài đặt thông báo cho Azure AD Kết nối Health. Vui lòng xem lại cài đặt của bạn. Hướng [dẫn này](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) có thể giúp bạn hiểu cách đặt cấu hình thiết đặt thông báo cho Azure AD và Kết nối thông báo tình trạng tốt.
- Để tìm hiểu thêm về báo cáo đồng bộ AAD Kết nối Health và cách tải xuống báo cáo, hãy xem Báo cáo đồng bộ [hóa mức đối tượng](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Để khắc phục sự cố cảnh báo Tình trạng AAD Kết nối, hãy làm theo hướng dẫn khắc phục sự cố cho cảnh báo làm mới dữ liệu [AAD Kết nối](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Tình trạng và đối với các câu hỏi thường gặp, hãy xem mục Câu hỏi cài đặt [AAD Kết nối](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)Tình trạng thường gặp.
