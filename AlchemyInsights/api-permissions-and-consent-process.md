---
title: Quyền API và quy trình chấp thuận
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405446"
---
# <a name="api-permissions-and-consent-process"></a><span data-ttu-id="5e0f8-102">Quyền API và quy trình chấp thuận</span><span class="sxs-lookup"><span data-stu-id="5e0f8-102">API Permissions and Consent Process</span></span>

<span data-ttu-id="5e0f8-103">Đối với ứng dụng của bạn để truy nhập dữ liệu trong Microsoft graph, người dùng hoặc người quản trị phải cấp quyền chính xác thông qua quy trình chấp thuận.</span><span class="sxs-lookup"><span data-stu-id="5e0f8-103">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="5e0f8-104">[Tham chiếu quyền đối với Microsoft graph](https://docs.microsoft.com/graph/permissions-reference) liệt kê các quyền liên kết với mỗi bộ các API chính của Microsoft graph.</span><span class="sxs-lookup"><span data-stu-id="5e0f8-104">[Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="5e0f8-105">Nó cũng cung cấp hướng dẫn về cách sử dụng các quyền.</span><span class="sxs-lookup"><span data-stu-id="5e0f8-105">It also provides guidance about how to use the permissions.</span></span>

<span data-ttu-id="5e0f8-106">**Thiết lập hoặc Cập Nhật hiệu trưởng dịch vụ**</span><span class="sxs-lookup"><span data-stu-id="5e0f8-106">**Set up or update service principal**</span></span>

- <span data-ttu-id="5e0f8-107">[Tạo hiệu trưởng](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) -bài viết này cho bạn biết cách tạo đối tượng dịch vụ mới.</span><span class="sxs-lookup"><span data-stu-id="5e0f8-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - This article shows you how to create a new servicePrincipal object.</span></span>
- <span data-ttu-id="5e0f8-108">[Tạo một AZURE AD app & dịch vụ chính trong cổng thông tin](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) -bài viết này cho bạn biết cách tạo ứng dụng Azure Active Directory (Azure AD) và hiệu trưởng dịch vụ có thể được sử dụng với điều khiển truy nhập dựa trên vai trò.</span><span class="sxs-lookup"><span data-stu-id="5e0f8-108">[Create an Azure AD app & service principal in the portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - This article shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
- <span data-ttu-id="5e0f8-109">Các [ứng dụng & hiệu trưởng dịch vụ trong AZURE AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) -bài viết này mô tả đăng ký ứng dụng, đối tượng ứng dụng và hiệu trưởng dịch vụ trong Azure Active Directory: chúng là gì, cách chúng được dùng và cách chúng liên quan đến nhau.</span><span class="sxs-lookup"><span data-stu-id="5e0f8-109">[Apps & service principals in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - This article describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span>

<span data-ttu-id="5e0f8-110">**Thêm hoặc cập nhật đăng ký ứng dụng và cung cấp sự đồng ý của người quản trị**</span><span class="sxs-lookup"><span data-stu-id="5e0f8-110">**Add or update app registration and provide admin consent**</span></span>

- <span data-ttu-id="5e0f8-111">[Tạo đăng ký ứng dụng](https://docs.microsoft.com/graph/api/application-post-applications) -bài viết này cho bạn biết cách tạo đối tượng ứng dụng mới.</span><span class="sxs-lookup"><span data-stu-id="5e0f8-111">[Create an app registration](https://docs.microsoft.com/graph/api/application-post-applications) - This article shows you how to create a new application object.</span></span>
- <span data-ttu-id="5e0f8-112">[Cập Nhật đăng ký ứng dụng-quyền API](https://docs.microsoft.com/graph/api/application-update) -bài viết này cho bạn biết cách cập nhật các thuộc tính của đối tượng ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="5e0f8-112">[Update an app registration - API permissions](https://docs.microsoft.com/graph/api/application-update) - This article shows you how to update the properties of an application object.</span></span>
- <span data-ttu-id="5e0f8-113">[Cung cấp sự chấp thuận quản trị](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) -chấp thuận và đồng ý người quản trị trong chung, chúng tôi yêu cầu người quản trị được cấp phép một cách rõ ràng.</span><span class="sxs-lookup"><span data-stu-id="5e0f8-113">[Provide admin consent](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - For admin consent and consent in general, we require that an admin explicitly grants consent.</span></span>
- <span data-ttu-id="5e0f8-114">Hàm [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) -bộ chứa quản lý vai trò cho các định nghĩa vai trò hợp nhất và gán vai trò cho các nhà cung cấp Microsoft 365 RBAC hỗ trợ nhiều hiệu trưởng và nhiều phạm vi trong một nhiệm vụ vai trò duy nhất.</span><span class="sxs-lookup"><span data-stu-id="5e0f8-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="5e0f8-115">Điều này khác với loại tài nguyên *Rbacapplication* .</span><span class="sxs-lookup"><span data-stu-id="5e0f8-115">This is different from *rbacApplication* resource type.</span></span> <span data-ttu-id="5e0f8-116">Microsoft InTune là một ví dụ về một nhà cung cấp RBAC như vậy.</span><span class="sxs-lookup"><span data-stu-id="5e0f8-116">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="5e0f8-117">Gán vai trò trong InTune có thể có một mảng hiệu trưởng và một mảng của các nhóm phạm vi.</span><span class="sxs-lookup"><span data-stu-id="5e0f8-117">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span> <span data-ttu-id="5e0f8-118">**Đây là trong phiên bản beta, có nghĩa là nó vẫn đang được phát triển và không được khuyên dùng để sử dụng trong sản xuất.**</span><span class="sxs-lookup"><span data-stu-id="5e0f8-118">**This is in beta, meaning that it is still in development and not recommended for use in production.**</span></span>
