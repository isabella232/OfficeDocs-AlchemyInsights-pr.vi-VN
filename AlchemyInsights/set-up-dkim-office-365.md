---
title: Thiết lập DKIM trong Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765561"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="d43b9-102">Thiết lập DKIM trong Office 365</span><span class="sxs-lookup"><span data-stu-id="d43b9-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="d43b9-103">Hướng dẫn đầy đủ cho các cấu hình DKIM cho các lĩnh vực tùy chỉnh trong Office 365 là [ở đây](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="d43b9-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="d43b9-104">Cho **mỗi** tên miền tuỳ chỉnh, bạn cần để tạo ra **hai** DKIM bản ghi CNAME tại tên miền của bạn dịch vụ lưu trữ DNS (thông thường, nhà cung cấp miền).</span><span class="sxs-lookup"><span data-stu-id="d43b9-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="d43b9-105">Ví dụ: contoso.com và fourthcoffee.com yêu cầu bốn ghi DKIM CNAME: hai cho contoso.com và hai cho fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="d43b9-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="d43b9-106">Bản ghi DKIM CNAME cho **mỗi** tên miền tuỳ chỉnh sử dụng định dạng sau:</span><span class="sxs-lookup"><span data-stu-id="d43b9-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="d43b9-107">**Tên máy chủ**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="d43b9-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="d43b9-108">**Điểm đến địa chỉ hoặc giá trị**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="d43b9-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="d43b9-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="d43b9-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="d43b9-110">**Tên máy chủ**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="d43b9-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="d43b9-111">**Điểm đến địa chỉ hoặc giá trị**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="d43b9-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="d43b9-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="d43b9-112">**TTL**: 3600</span></span>

   <span data-ttu-id="d43b9-113">\<DomainGUID\> văn bản bên trái của `.mail.protection.outlook.com` trong bản ghi MX tùy chỉnh tùy chỉnh tên miền (ví dụ, `contoso-com` cho miền contoso.com).</span><span class="sxs-lookup"><span data-stu-id="d43b9-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="d43b9-114">\<InitialDomain\> là tên miền bạn đã sử dụng khi đăng ký Office 365 (ví dụ, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="d43b9-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="d43b9-115">Sau khi bạn đã tạo bản ghi CNAME cho miền của bạn tùy chỉnh, đầy đủ các hướng dẫn sau:</span><span class="sxs-lookup"><span data-stu-id="d43b9-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="d43b9-116">một.</span><span class="sxs-lookup"><span data-stu-id="d43b9-116">a.</span></span> <span data-ttu-id="d43b9-117">[Đăng nhập Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) với tài khoản của bạn làm việc hoặc trường học.</span><span class="sxs-lookup"><span data-stu-id="d43b9-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="d43b9-118">b.</span><span class="sxs-lookup"><span data-stu-id="d43b9-118">b.</span></span> <span data-ttu-id="d43b9-119">Chọn biểu tượng phóng ứng dụng ở trên bên trái và chọn **Admin**.</span><span class="sxs-lookup"><span data-stu-id="d43b9-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="d43b9-120">c.</span><span class="sxs-lookup"><span data-stu-id="d43b9-120">c.</span></span> <span data-ttu-id="d43b9-121">Điều hướng dưới bên trái, mở rộng các **Admin** và chọn **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="d43b9-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="d43b9-122">d.</span><span class="sxs-lookup"><span data-stu-id="d43b9-122">d.</span></span> <span data-ttu-id="d43b9-123">Đi để **bảo vệ** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="d43b9-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="d43b9-124">e.</span><span class="sxs-lookup"><span data-stu-id="d43b9-124">e.</span></span> <span data-ttu-id="d43b9-125">Chọn tên miền và sau đó chọn **sử** **ký**thư cho miền này với DKIM chữ ký.</span><span class="sxs-lookup"><span data-stu-id="d43b9-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="d43b9-126">Lặp lại bước này cho mỗi tên miền tuỳ chỉnh.</span><span class="sxs-lookup"><span data-stu-id="d43b9-126">Repeat this step for each custom domain.</span></span>
