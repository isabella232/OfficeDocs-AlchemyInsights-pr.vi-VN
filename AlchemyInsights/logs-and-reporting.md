---
title: Nhật ký và báo cáo
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036102"
---
# <a name="logs-and-reporting"></a>Nhật ký và báo cáo

Câu hỏi [thường gặp về Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) câu hỏi thường gặp về báo cáo Azure Active Directory (Azure AD). Để biết thêm thông tin, hãy xem [báo cáo Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).

**Khắc phục sự cố về kiểm tra**

1. Nếu bạn đang gặp vấn đề khi thấy một số hoạt động kiểm nghiệm và hoạt động bị thiếu nằm trong [danh sách](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)này, vui lòng gửi một vé hỗ trợ.
2. Nếu bạn đang gặp vấn đề khi thấy bất kỳ Nhật ký kiểm tra nào trong đối tượng thuê của mình, vui lòng gửi một vé hỗ trợ.
3. Nếu các hoạt động kiểm nghiệm của bạn không hiển thị ngay lập tức trong cổng thông tin Azure, hãy xem [thông tin về độ trễ](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) của chúng tôi và gửi một vé hỗ trợ nếu sự chậm trễ vượt quá độ trễ của tài liệu.
4. [Duy trì ghi nhật ký hoạt động Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. Nếu bạn không nhìn thấy tất cả kiểm nghiệm cho phạm vi ngày bạn đã chọn, bạn có thể tải lên đến 250K hàng (được sắp xếp theo gần đây nhất) của các đăng nhập từ Azure Portal. Để biết thêm thông tin, hãy xem [tải xuống các hoạt động kiểm](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)nghiệm.

**Khắc phục sự cố với đăng nhập**

1. Bạn chỉ có thể nhìn thấy 30 ngày cuối cùng của dữ liệu nếu bạn có giấy phép Azure AD Premium (P1 hoặc P2) cho đối tượng thuê của bạn.
2. Đăng nhập chỉ khả dụng cho các đối tượng thuê Azure AD Premium. Nó không sẵn dùng đối với người thuê cơ bản miễn phí hoặc được cấp phép.
3. Nếu đối tượng thuê của bạn có giấy phép P1 Premium và bạn không nhìn thấy các đăng nhập, hãy kiểm tra [thông tin về độ trễ](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) của chúng tôi và gửi một vé hỗ trợ nếu sự chậm trễ vượt quá độ trễ tài liệu.
4. Nếu bạn không nhìn thấy tất cả các đăng nhập cho phạm vi ngày bạn đã chọn, hãy lưu ý rằng bạn có thể tải lên đến 250K hàng (được sắp xếp theo gần đây nhất) của các đăng nhập từ Azure Portal. Để biết thêm thông tin, hãy xem [tải xuống các hoạt động đăng nhập](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).

**Khắc phục sự cố báo cáo bảo mật (người dùng gắn cờ có nguy cơ, đăng nhập rủi ro)**

1. [Người dùng gắn cờ cho báo cáo bảo mật rủi ro](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [Báo cáo đăng nhập rủi ro trong cổng thông tin Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [Sự kiện rủi ro trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
