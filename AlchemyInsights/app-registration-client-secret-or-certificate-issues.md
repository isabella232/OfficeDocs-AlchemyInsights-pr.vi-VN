---
title: Các vấn đề của máy khách đăng ký ứng dụng hoặc chứng chỉ
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
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405327"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="f8025-102">Các vấn đề của máy khách đăng ký ứng dụng hoặc chứng chỉ</span><span class="sxs-lookup"><span data-stu-id="f8025-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="f8025-103">Ứng dụng khách hàng bí mật hết hạn?</span><span class="sxs-lookup"><span data-stu-id="f8025-103">Application client secret expiring?</span></span>

<span data-ttu-id="f8025-104">Bất kể ứng dụng đã đăng ký như thế nào được tạo ra, cho dù thông qua quy trình đăng ký chuẩn trong cổng đăng ký ứng dụng hay nếu hiệu trưởng dịch vụ được tạo ra trong đối tượng thuê của bạn bằng sự đồng ý của ứng dụng, một bí mật khách hàng mới sẽ cần được tạo trước khi hết thời hạn hiện tại và Cập Nhật trong mã ứng dụng liên quan.</span><span class="sxs-lookup"><span data-stu-id="f8025-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="f8025-105">Khoảng thời gian có hiệu lực tối đa là 2 năm.</span><span class="sxs-lookup"><span data-stu-id="f8025-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="f8025-106">Với tư cách là lời nhắc giá trị bí mật phải được ghi lại vì nó sẽ không còn hiển thị sau khi rời khỏi trang đăng ký ứng dụng trong cổng thông tin.</span><span class="sxs-lookup"><span data-stu-id="f8025-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="f8025-107">Để biết thêm thông tin, hãy xem [bắt đầu nhanh: đăng ký ứng dụng trong nền tảng định danh Microsoft](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) và [các cách thực hành tốt nhất cho nền tảng định danh Microsoft](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span><span class="sxs-lookup"><span data-stu-id="f8025-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="f8025-108">Để tìm hiểu thêm, hãy xem [tạo ứng dụng AZURE AD & hiệu trưởng dịch vụ trong cổng thông tin-Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span><span class="sxs-lookup"><span data-stu-id="f8025-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
