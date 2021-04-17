---
title: Chính sách truy nhập có điều kiện
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: af95627d07d41add54f03c9254562b9be4e05d9b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817302"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="de30b-102">Chính sách truy nhập có điều kiện</span><span class="sxs-lookup"><span data-stu-id="de30b-102">Conditional Access policies</span></span>

<span data-ttu-id="de30b-103">Quyền truy nhập có điều kiện là một khả năng của Azure AD cho phép bạn thực thi các điều khiển trên quyền truy nhập vào các ứng dụng trong môi trường của mình, tất cả đều dựa trên các điều kiện cụ thể và được quản lý từ vị trí trung tâm.</span><span class="sxs-lookup"><span data-stu-id="de30b-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="de30b-104">Tìm hiểu thêm về [AZURE AD Access](https://docs.microsoft.com/azure/active-directory/conditional-access/)có điều kiện.</span><span class="sxs-lookup"><span data-stu-id="de30b-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="de30b-105">**Lưu ý**: nếu đối tượng thuê của bạn đã được tạo sau ngày 21 tháng 10, 2019 và bạn đang gặp phải lời nhắc MFA, có thể bạn đã bật tính năng [mặc định bảo mật](https://aka.ms/securitydefaults) trong đối tượng thuê của mình.</span><span class="sxs-lookup"><span data-stu-id="de30b-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="de30b-106">**Để quản lý mặc định bảo mật**</span><span class="sxs-lookup"><span data-stu-id="de30b-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="de30b-107">Đăng nhập vào [Trung tâm quản trị](https://go.microsoft.com/fwlink/p/?linkid=834822) bằng thông tin xác thực người quản trị toàn cầu của bạn.</span><span class="sxs-lookup"><span data-stu-id="de30b-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="de30b-108">Truy nhập vào [thuộc tính Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="de30b-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="de30b-109">Ở cuối trang, hãy bấm **quản lý mặc định bảo mật**.</span><span class="sxs-lookup"><span data-stu-id="de30b-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="de30b-110">Bấm **có** để cho phép mặc định bảo mật hoặc **không** tắt tính năng mặc định bảo mật.</span><span class="sxs-lookup"><span data-stu-id="de30b-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
