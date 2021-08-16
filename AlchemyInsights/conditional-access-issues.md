---
title: Các sự cố truy nhập có điều kiện
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069986"
---
# <a name="conditional-access-issues"></a>Các sự cố truy nhập có điều kiện

**Giải quyết các vấn đề với Chẩn đoán Đăng nhập**

Bạn có thể nhanh chóng tìm ra sự cố đã xảy ra hoặc chẩn đoán sự cố liên quan đến đăng nhập người dùng bằng [cách sử dụng Chẩn đoán Đăng nhập:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Khởi chạy Chẩn đoán Đăng nhập.
1. Tìm sự kiện cần phân tích bằng cách nhập các chi tiết mà bạn có về người dùng, ứng dụng, thời gian đăng nhập, yêu cầu Id hoặc Id tương quan.
1. Xem lại kết quả chẩn đoán hiển thị chi tiết sự cố đã xảy ra và những hành động bạn có thể thực hiện để thực hiện thay đổi (nếu cần bất kỳ thay đổi nào).

**Các bước khắc phục sự cố đăng nhập** 

1. Dẫn hướng đến trang Đăng nhập Azure AD.
1. Lọc đăng nhập theo người dùng, phạm vi thời gian, ứng dụng, trạng thái, ứng dụng máy khách, v.v.
1. Chọn một sự kiện đăng nhập và xem tab Truy nhập có Điều kiện để xem những chính sách nào đã được đánh giá.
1. Bấm vào hàng của chính sách để xem chi tiết chính sách và tìm hiểu lý do chính sách được áp dụng.

**Công cụ để khắc phục sự cố chính sách Truy nhập có Điều kiện**

- Chế độ chỉ báo cáo cho phép bạn đánh giá một chính sách mà không làm ảnh hưởng đến người dùng.
- Công cụ tình thế nếu-xảy-ra cho phép bạn mô phỏng các sự kiện đăng nhập và xem chính sách nào được áp dụng.
- Insights việc báo cáo và sổ làm việc hiển thị ảnh hưởng theo thời gian thực của từng chính sách.

**Chính sách Bảo vệ Đường cơ sở**

Các chính sách Bảo vệ Đường cơ sở đã bị không còn sử dụng nữa. Chúng sẽ không còn được thực thi nữa và sẽ sớm bị loại bỏ khỏi cổng thông tin Azure. Chúng tôi khuyên bạn nên [bật các mặc định bảo mật.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Để biết thêm thông tin về Truy nhập có điều kiện, hãy xem:

[Cách thực hành tốt nhất cho truy nhập có điều kiện trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Các điều kiện trong Truy nhập có điều kiện](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Các điều khiển trong Truy nhập có điều kiện](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Các vị trí trong truy cập có điều kiện](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
