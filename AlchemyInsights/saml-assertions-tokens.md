---
title: Các khẳng định SAML (thẻ)
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
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885783"
---
# <a name="saml-assertions-tokens"></a>Các khẳng định SAML (thẻ)

1. Các thẻ ngôn ngữ đánh dấu sự khẳng định bảo mật (SAML) là biểu thị XML của tuyên bố. Theo mặc định, hãy dùng thẻ trao đổi Windows Communication Foundation (WCF) trong các tình huống bảo mật được liên kết được phát hành. Để biết thêm thông tin, hãy xem [thẻ SAML và tuyên bố](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Nền tảng Microsoft Identity phát ra một số loại thẻ bảo mật trong quá trình xử lý mỗi dòng xác thực. [Tham chiếu tuyên bố mã thông báo SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) mô tả định dạng, đặc tính bảo mật và nội dung của các thẻ 2,0.
3. Làm theo hướng dẫn trong [hạn cấu hình mã thông báo trong Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) để tìm hiểu cách cấu hình hạn của token.
4. Làm theo các bước được nêu trong [bài viết này](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) để tìm hiểu cách cấu hình mã hóa mã thông báo AZURE AD SAML.
5. Trong Azure AD, bạn có thể thiết lập các tùy chọn ký chứng chỉ và thuật toán ký chứng chỉ. Để biết thêm thông tin, hãy xem [các tùy chọn ký chứng chỉ nâng cao trong các ứng dụng bộ sưu tập mã thông báo SAML trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
