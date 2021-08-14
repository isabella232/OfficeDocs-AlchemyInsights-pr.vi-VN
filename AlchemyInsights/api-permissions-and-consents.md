---
title: Quyền và Sự chấp thuận API
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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932119"
---
# <a name="api-permissions-and-consent"></a>Quyền và sự chấp thuận API

Các ứng dụng tích hợp với Nền tảng định danh Microsoft theo mô hình ủy quyền cho phép người dùng và người quản trị kiểm soát cách truy nhập dữ liệu. Việc triển khai mô hình ủy quyền đã được cập nhật trên Nền tảng định danh Microsoft cuối. Nó thay đổi cách ứng dụng phải tương tác với thư Nền tảng định danh Microsoft. [Các quyền và sự chấp thuận trong điểm cuối Nền tảng định danh Microsoft bao](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) gồm các khái niệm cơ bản của mô hình ủy quyền này, bao gồm phạm vi, quyền và sự chấp thuận.

Khuôn [khổ chấp Azure Active Directory dụng (Azure AD) giúp](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) dễ dàng phát triển các ứng dụng web nhiều đối tượng thuê và máy khách gốc. Những ứng dụng này cho phép đăng nhập bằng tài khoản người dùng từ đối tượng thuê Azure AD khác với đối tượng thuê đã đăng ký ứng dụng. Họ cũng có thể cần truy nhập các API web như API Microsoft Graph (để truy nhập Azure AD, Intune và các dịch vụ trong Microsoft 365) và các API khác của dịch vụ Microsoft, ngoài các API web của riêng bạn.

