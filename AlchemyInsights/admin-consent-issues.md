---
title: Sự đồng ý của người quản trị vấn đề
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901517"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="d4a5e-102">Sự đồng ý của người quản trị vấn đề</span><span class="sxs-lookup"><span data-stu-id="d4a5e-102">Admin consent issues</span></span>

1. <span data-ttu-id="d4a5e-103">Bật dòng công việc [chấp thuận quản trị](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) để cho phép người dùng yêu cầu phê duyệt người quản trị trực tiếp từ màn hình chấp thuận.</span><span class="sxs-lookup"><span data-stu-id="d4a5e-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="d4a5e-104">Nếu bạn hoặc người dùng ứng dụng của bạn đang gặp phải lỗi không mong muốn trong quá trình chấp thuận, hãy xem bài viết này để biết các bước khắc phục sự cố: [lỗi không mong muốn khi thực hiện việc đồng ý với một ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="d4a5e-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="d4a5e-105">Tìm hiểu thêm về [sự đồng ý của người quản trị trên nền tảng Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), cách [đồng ý nhắc](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) công việc và cách [đánh giá yêu cầu cho sự đồng ý của người quản trị đối tượng thuê](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="d4a5e-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="d4a5e-106">Các ứng dụng tích hợp với nền tảng định danh Microsoft theo dõi một mô hình ủy quyền cung cấp cho người dùng và người quản trị kiểm soát dữ liệu có thể truy nhập như thế nào.</span><span class="sxs-lookup"><span data-stu-id="d4a5e-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="d4a5e-107">Việc thực hiện mô hình ủy quyền đã được Cập Nhật trên điểm cuối Microsoft Identity Platform và thay đổi cách ứng dụng phải tương tác với nền tảng định danh Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d4a5e-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="d4a5e-108">Xem [các quyền và sự đồng ý trong điểm cuối Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) để biết tổng quan về mô hình ủy quyền này, bao gồm phạm vi, quyền và đồng ý.</span><span class="sxs-lookup"><span data-stu-id="d4a5e-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>