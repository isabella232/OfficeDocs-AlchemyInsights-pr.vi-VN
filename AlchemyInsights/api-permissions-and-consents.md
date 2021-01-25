---
title: Quyền API và sự đồng ý
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
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974999"
---
# <a name="api-permissions-and-consent"></a>Quyền API và sự đồng ý

Các ứng dụng tích hợp với nền tảng định danh Microsoft theo dõi một mô hình ủy quyền cung cấp cho người dùng và người quản trị kiểm soát dữ liệu có thể truy nhập như thế nào. Việc thực hiện mô hình ủy quyền đã được Cập Nhật trên điểm cuối Microsoft Identity Platform. Nó thay đổi cách ứng dụng phải tương tác với nền tảng định danh Microsoft. [Quyền và sự đồng ý trong điểm cuối Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) bao gồm các khái niệm cơ bản về mô hình ủy quyền này, bao gồm phạm vi, quyền và đồng ý.

[Khuôn khổ thỏa thuận Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) giúp bạn dễ dàng phát triển web nhiều đối tượng thuê và các ứng dụng máy khách gốc. Những ứng dụng này cho phép đăng nhập bằng tài khoản người dùng từ một đối tượng thuê Azure quảng cáo khác nhau từ một nơi mà ứng dụng đã đăng ký. Họ cũng có thể cần truy nhập các API web như API của Microsoft graph (để truy nhập Azure AD, InTune và các dịch vụ trong Microsoft 365) và các API khác của Microsoft Services, ngoài các API web của riêng bạn.

