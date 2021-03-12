---
title: Các vấn đề với người thuê
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7824"
- "9004325"
ms.openlocfilehash: 43f75564667bbb952076d4c12d7a1dd1e7e99731
ms.sourcegitcommit: 4e2d640a618c786700e8b276533554d51956f080
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714480"
---
# <a name="issues-with-tenants"></a><span data-ttu-id="72895-102">Các vấn đề với người thuê</span><span class="sxs-lookup"><span data-stu-id="72895-102">Issues with tenants</span></span>

<span data-ttu-id="72895-103">Azure Active Directory (Azure AD) tổ chức các đối tượng như người dùng và ứng dụng thành các nhóm có tên là đối tượng thuê.</span><span class="sxs-lookup"><span data-stu-id="72895-103">Azure Active Directory (Azure AD) organizes objects like users and apps into groups called tenants.</span></span> <span data-ttu-id="72895-104">Đối tượng thuê cho phép người quản trị đặt chính sách trên người dùng trong tổ chức và trên các ứng dụng mà tổ chức sở hữu để đáp ứng các chính sách bảo mật và hoạt động của họ.</span><span class="sxs-lookup"><span data-stu-id="72895-104">Tenants allow an administrator to set policies on the users within the organization and the on apps that the organization owns to meet their security and operational policies.</span></span> <span data-ttu-id="72895-105">Để biết thêm thông tin, hãy xem mục ghi nhớ [trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/single-and-multi-tenant-apps).</span><span class="sxs-lookup"><span data-stu-id="72895-105">For more information, see [Tenancy in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/single-and-multi-tenant-apps).</span></span>

<span data-ttu-id="72895-106">Để biết thêm thông tin liên quan đến quản lý đối tượng thuê, hãy xem các bài viết sau đây:</span><span class="sxs-lookup"><span data-stu-id="72895-106">For more information related to tenant management, see the following articles:</span></span>

- <span data-ttu-id="72895-107">[Bắt đầu nhanh: thiết lập một](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant) đối tượng thuê-cho bạn biết cách tạo một đối tượng thuê mới.</span><span class="sxs-lookup"><span data-stu-id="72895-107">[Quickstart: Set up a tenant](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant) - Shows you how to create a new tenant.</span></span>

- <span data-ttu-id="72895-108">[Xóa một đối tượng thuê trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto) -cho bạn biết cách xóa một đối tượng thuê.</span><span class="sxs-lookup"><span data-stu-id="72895-108">[Delete a tenant in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto) - Shows you how to delete a tenant.</span></span>

<span data-ttu-id="72895-109">**Các vấn đề với nhiều người thuê**</span><span class="sxs-lookup"><span data-stu-id="72895-109">**Issues with multi-tenants**</span></span>

<span data-ttu-id="72895-110">Để biết thêm thông tin về cách quản lý các vấn đề về nhiều người thuê, hãy xem các bài viết sau đây:</span><span class="sxs-lookup"><span data-stu-id="72895-110">For information on how to manage issues regarding multi-tenants, see the following articles:</span></span>

- <span data-ttu-id="72895-111">[Cách: đăng nhập vào bất kỳ người dùng Azure Active Directory nào bằng mẫu ứng dụng nhiều](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant) đối tượng thuê-cho bạn biết cách chuyển đổi từ một đối tượng thuê riêng cho một ứng dụng nhiều đối tượng thuê.</span><span class="sxs-lookup"><span data-stu-id="72895-111">[How to: Sign in any Azure Active Directory user using the multi-tenant application pattern](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant) - Shows you how to convert from a single-tenant to a multi-tenant application.</span></span>
- <span data-ttu-id="72895-112">[Thiết lập đăng nhập cho một tổ chức Azure Active Directory cụ thể trong Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-single-tenant?pivots=b2c-user-flow) -cho bạn biết cách cho phép đăng nhập cho người dùng từ một tổ chức Azure AD cụ thể bằng cách sử dụng dòng người dùng trong AZURE AD B2C.</span><span class="sxs-lookup"><span data-stu-id="72895-112">[Set up sign-in for a specific Azure Active Directory organization in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-single-tenant?pivots=b2c-user-flow) - Shows you how to enable sign-in for users from a specific Azure AD organization using a user flow in Azure AD B2C.</span></span>
- <span data-ttu-id="72895-113">[Thiết lập đăng nhập cho nhiều đối tượng thuê Azure Active Directory bằng chính sách tùy chỉnh trong Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-multi-tenant?pivots=b2c-custom-policy)  cho bạn biết cách cho phép đăng nhập cho người dùng bằng cách sử dụng điểm cuối nhiều đối tượng thuê cho Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="72895-113">[Set up sign-in for multi-tenant Azure Active Directory using custom policies in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-multi-tenant?pivots=b2c-custom-policy)  shows you how to enable sign-in for users using the multi-tenant endpoint for Azure Active Directory (Azure AD).</span></span>






