---
title: Các vấn đề truy nhập có điều kiện
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
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015007"
---
# <a name="conditional-access-issues"></a>Các vấn đề truy nhập có điều kiện

**Giải quyết vấn đề khi chẩn đoán đăng nhập**

Bạn có thể nhanh chóng tìm hiểu điều gì đã xảy ra hoặc chẩn đoán các vấn đề liên quan đến người dùng đăng nhập bằng cách sử dụng [chẩn đoán đăng nhập](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. Khởi động chẩn đoán đăng nhập.
1. Tìm sự kiện để phân tích bằng cách nhập vào các chi tiết bạn có về người dùng, ứng dụng, thời gian đăng nhập, yêu cầu ID hoặc tương quan ID.
1. Xem lại kết quả chẩn đoán Hiển thị chi tiết về những điều đã xảy ra và những hành động bạn có thể thực hiện để thay đổi (nếu có bất kỳ thay đổi nào cần thiết).

**Các bước để khắc phục sự cố đăng nhập** 

1. Dẫn hướng đến trang đăng nhập Azure AD.
1. Lọc đăng nhập bằng người dùng, phạm vi thời gian, ứng dụng, trạng thái, ứng dụng khách, v.v.
1. Chọn sự kiện đăng nhập và xem tab truy nhập có điều kiện để xem các chính sách nào được đánh giá.
1. Bấm vào hàng của chính sách để xem chi tiết chính sách và hiểu tại sao nó được áp dụng.

**Công cụ để khắc phục sự cố chính sách truy nhập có điều kiện**

- Chế độ chỉ báo cáo cho phép bạn đánh giá chính sách mà không tác động đến người dùng.
- Công cụ điều gì sẽ cho phép bạn mô phỏng các sự kiện đăng nhập và xem các chính sách nào sẽ áp dụng.
- Sổ làm việc hiểu biết và báo cáo hiển thị ảnh hưởng theo thời gian thực của mỗi chính sách.

**Chính sách bảo vệ đường cơ sở**

Các chính sách bảo vệ đường cơ sở đã bị suy giảm. Chúng không còn được áp thi và sẽ sớm được loại bỏ khỏi Azure Portal. Chúng tôi khuyên bạn nên bật tính năng [mặc định bảo mật](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Để biết thêm thông tin về truy nhập có điều kiện, hãy xem:

Các cách [thực hành tốt nhất để truy nhập có điều kiện trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 Các [điều kiện trong quyền truy nhập](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 có điều kiện [Điều khiển trong quyền truy nhập](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 có điều kiện [Vị trí trong Access](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition) có điều kiện
