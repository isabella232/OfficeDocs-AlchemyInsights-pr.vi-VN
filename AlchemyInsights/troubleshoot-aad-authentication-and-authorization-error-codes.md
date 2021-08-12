---
title: Khắc phục sự cố mã lỗi Xác thực và Ủy quyền Azure AD (AADSTS)
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
ms.openlocfilehash: ac25548b0110834c877ae53be097d6b6c0f13c4091040a901abd56fb2a3cbba3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939977"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Khắc phục sự cố mã lỗi Xác thực và Ủy quyền Azure AD (AADSTS)

Để giải quyết mã lỗi xác thực và ủy quyền AAD (AADSTS), hãy thực hiện các bước được đề xuất sau đây:

1. **Xử lý mã lỗi trong ứng dụng của bạn**

- Thông **số OAuth2.0**, cung cấp hướng dẫn về cách xử lý lỗi trong quá trình xác thực bằng cách https://tools.ietf.org/html/rfc6749#section-5.2 dùng phần lỗi trong phản hồi lỗi.

    - **:** Một chuỗi mã lỗi có thể được dùng để phân loại các loại lỗi xảy ra và sẽ được dùng để phản ứng với lỗi.
    - Trường  lỗi có một vài giá trị có thể xảy ra - xem lại các liên kết hướng dẫn sử dụng giao thức và thông số OAuth 2.0 để biết thêm thông tin về các lỗi cụ thể và cách phản hồi các lỗi đó.

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

- Mã lỗi và thông báo có thể thay đổi. Để biết thông tin mới nhất, hãy xem trang để tìm mô tả lỗi AADSTS, các bản sửa lỗi và một số giải pháp https://login.microsoftonline.com/error thay thế được đề xuất.
- Bạn cũng có thể tìm kiếm và khắc phục sự cố mã [lỗi AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) được liệt kê trong bài viết [Azure AD Authentication và mã lỗi ủy quyền.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)

3. **Nhận trợ giúp**

- Các tùy chọn hỗ trợ và trợ giúp dành cho nhà phát triển [-](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) Nếu bạn cần câu trả lời cho một câu hỏi hoặc trợ giúp trong việc giải quyết một vấn đề không có trong tài liệu của chúng tôi, đã đến lúc phải liên hệ với các chuyên gia để được trợ giúp. Bài viết này cung cấp một số gợi ý để nhận câu trả lời cho câu hỏi của bạn khi bạn phát triển ứng dụng tích hợp với Nền tảng định danh Microsoft.








