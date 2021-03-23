---
title: Khắc phục sự cố mã lỗi xác thực và ủy quyền của Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037844"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Khắc phục sự cố mã lỗi xác thực và ủy quyền của Azure AD

Để giải quyết xác thực và mã lỗi ủy quyền, hãy thực hiện các bước được đề xuất sau đây:

1. **Mã lỗi xử lý trong ứng dụng của bạn**

- **Spec OAuth 2.0**, https://tools.ietf.org/html/rfc6749#section-5.2 , cung cấp hướng dẫn về cách xử lý lỗi trong khi xác thực bằng cách dùng phần lỗi của phản hồi lỗi.

    - **lỗi**: một chuỗi mã lỗi có thể được dùng để phân loại các kiểu lỗi xảy ra và được dùng để phản đối lỗi.
    - Trường **lỗi** có một số giá trị có thể xem lại các nối kết tài liệu hướng dẫn giao thức và ứng dụng web oauth 2,0 để biết thêm thông tin về các lỗi cụ thể và cách phản đối cho chúng.

- Đây là một phản hồi lỗi mẫu:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Tra cứu thông tin mã lỗi hiện tại**

- Mã lỗi và thư có thể thay đổi. Để biết thông tin mới nhất, hãy xem https://login.microsoftonline.com/error trang để tìm hiểu về mô tả lỗi, bản sửa lỗi và một số giải pháp thay thế được gợi ý.
- Bạn cũng có thể tìm kiếm và khắc phục sự cố các [mã lỗi](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) được liệt kê trong bài viết [Azure AD Authentication và các mã lỗi ủy quyền](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Nhận trợ giúp**

- [Tùy chọn hỗ trợ và trợ giúp dành cho nhà phát triển](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) -nếu bạn cần câu trả lời cho câu hỏi hoặc trợ giúp trong việc giải quyết sự cố không được bảo hiểm trong tài liệu của chúng tôi, có thể là thời gian để tiếp cận với các chuyên gia để được trợ giúp. Bài viết này cung cấp một số gợi ý để nhận câu trả lời cho các câu hỏi của bạn khi bạn phát triển các ứng dụng tích hợp với nền tảng định danh Microsoft.








