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
# <a name="saml-assertions-tokens"></a><span data-ttu-id="eb205-102">Các khẳng định SAML (thẻ)</span><span class="sxs-lookup"><span data-stu-id="eb205-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="eb205-103">Các thẻ ngôn ngữ đánh dấu sự khẳng định bảo mật (SAML) là biểu thị XML của tuyên bố.</span><span class="sxs-lookup"><span data-stu-id="eb205-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="eb205-104">Theo mặc định, hãy dùng thẻ trao đổi Windows Communication Foundation (WCF) trong các tình huống bảo mật được liên kết được phát hành.</span><span class="sxs-lookup"><span data-stu-id="eb205-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="eb205-105">Để biết thêm thông tin, hãy xem [thẻ SAML và tuyên bố](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span><span class="sxs-lookup"><span data-stu-id="eb205-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="eb205-106">Nền tảng Microsoft Identity phát ra một số loại thẻ bảo mật trong quá trình xử lý mỗi dòng xác thực.</span><span class="sxs-lookup"><span data-stu-id="eb205-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="eb205-107">[Tham chiếu tuyên bố mã thông báo SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) mô tả định dạng, đặc tính bảo mật và nội dung của các thẻ 2,0.</span><span class="sxs-lookup"><span data-stu-id="eb205-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="eb205-108">Làm theo hướng dẫn trong [hạn cấu hình mã thông báo trong Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) để tìm hiểu cách cấu hình hạn của token.</span><span class="sxs-lookup"><span data-stu-id="eb205-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="eb205-109">Làm theo các bước được nêu trong [bài viết này](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) để tìm hiểu cách cấu hình mã hóa mã thông báo AZURE AD SAML.</span><span class="sxs-lookup"><span data-stu-id="eb205-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="eb205-110">Trong Azure AD, bạn có thể thiết lập các tùy chọn ký chứng chỉ và thuật toán ký chứng chỉ.</span><span class="sxs-lookup"><span data-stu-id="eb205-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="eb205-111">Để biết thêm thông tin, hãy xem [các tùy chọn ký chứng chỉ nâng cao trong các ứng dụng bộ sưu tập mã thông báo SAML trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="eb205-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
