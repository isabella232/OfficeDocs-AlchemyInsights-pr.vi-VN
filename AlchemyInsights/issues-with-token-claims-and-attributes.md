---
title: Các vấn đề với yêu cầu và thuộc tính mã thông báo
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036082"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="7f4bf-102">Các vấn đề với yêu cầu và thuộc tính mã thông báo</span><span class="sxs-lookup"><span data-stu-id="7f4bf-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="7f4bf-103">**Cập Nhật, cấu hình hoặc loại bỏ yêu cầu mã thông báo**</span><span class="sxs-lookup"><span data-stu-id="7f4bf-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="7f4bf-104">Bằng cách sử dụng Azure Active Directory (Azure AD), bạn có thể [tùy chỉnh kiểu yêu cầu bồi thường của vai trò](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) trong mã thông báo phản hồi mà bạn nhận được sau khi bạn ủy quyền cho một ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="7f4bf-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="7f4bf-105">Các nhà phát triển ứng dụng có thể sử dụng các tuyên bố tùy chọn trong ứng dụng Azure AD của họ để xác định những tuyên bố mà họ muốn trong thẻ được gửi đến ứng dụng của họ.</span><span class="sxs-lookup"><span data-stu-id="7f4bf-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="7f4bf-106">Để biết thêm thông tin, hãy xem [cung cấp tuyên bố tùy chọn vào ứng dụng của bạn](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="7f4bf-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="7f4bf-107">[Cấu hình tuyên bố nhóm cho các ứng dụng với Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span><span class="sxs-lookup"><span data-stu-id="7f4bf-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="7f4bf-108">Nếu dùng đăng nhập đơn seamless trong ứng dụng của bạn, hãy xem [tùy chỉnh tuyên bố phát hành trong các ứng dụng thông báo thông báo của doanh nghiệp SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span><span class="sxs-lookup"><span data-stu-id="7f4bf-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="7f4bf-109">**Lập bản đồ thuộc tính tuyên bố**</span><span class="sxs-lookup"><span data-stu-id="7f4bf-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="7f4bf-110">Để cấu hình chính sách ánh xạ tuyên bố bằng PowerShell, hãy xem [tùy chỉnh tuyên bố phát ra bằng thẻ cho một ứng dụng cụ thể trong một đối tượng thuê (bản xem trước)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="7f4bf-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="7f4bf-111">Thuộc tính Schema của phần mở rộng thư mục cung cấp cách để lưu trữ dữ liệu bổ sung trong Azure Active Directory trên đối tượng người dùng và các đối tượng thư mục khác chẳng hạn như nhóm, chi tiết đối tượng thuê, hiệu trưởng dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="7f4bf-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="7f4bf-112">Chỉ các thuộc tính phần mở rộng trên đối tượng người dùng có thể được sử dụng để phát ra các yêu cầu cho các ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="7f4bf-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="7f4bf-113">[Sử dụng các thuộc tính phần mở rộng của sơ đồ trong thư mục trong yêu cầu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) mô tả cách sử dụng thuộc tính phần mở rộng sơ đồ danh mục để gửi dữ liệu người dùng đến các ứng dụng trong yêu cầu</span><span class="sxs-lookup"><span data-stu-id="7f4bf-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="7f4bf-114">Để biết thêm thông tin về các yêu cầu token, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="7f4bf-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="7f4bf-115">Tuyên bố trong thẻ Access</span><span class="sxs-lookup"><span data-stu-id="7f4bf-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="7f4bf-116">Khiếu nại trong một id_token</span><span class="sxs-lookup"><span data-stu-id="7f4bf-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="7f4bf-117">[Tuyên bố](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) rằng bạn có thể trông đợi trong thẻ ID và thẻ Access do AZURE AD B2C phát hành</span><span class="sxs-lookup"><span data-stu-id="7f4bf-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="7f4bf-118">Tham khảo tuyên bố mã thông báo SAML</span><span class="sxs-lookup"><span data-stu-id="7f4bf-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
