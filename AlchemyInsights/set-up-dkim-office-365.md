---
title: Thiết lập DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509406"
---
# <a name="setup-dkim"></a><span data-ttu-id="219ae-102">Thiết lập DKIM</span><span class="sxs-lookup"><span data-stu-id="219ae-102">Setup DKIM</span></span>

<span data-ttu-id="219ae-103">Hướng dẫn đầy đủ để cấu hình DKIM cho tuỳ chỉnh miền trong Microsoft 365 đang [ở đây](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="219ae-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="219ae-104">Đối với **mỗi** miền tùy chỉnh, bạn cần tạo **hai** bản ghi DKIM CNAME tại dịch vụ lưu trữ DNS của miền (thông thường là công ty đăng ký tên miền).</span><span class="sxs-lookup"><span data-stu-id="219ae-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="219ae-105">Ví dụ, contoso.com và fourthcoffee.com yêu cầu bốn bản ghi DKIM CNAME: hai cho contoso.com và hai cho fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="219ae-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="219ae-106">Bản ghi DKIM CNAME cho **mỗi** miền tùy chỉnh sử dụng các định dạng sau:</span><span class="sxs-lookup"><span data-stu-id="219ae-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="219ae-107">**Tên máy chủ**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="219ae-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="219ae-108">**Điểm đến địa chỉ hoặc giá trị**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="219ae-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="219ae-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="219ae-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="219ae-110">**Tên máy chủ**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="219ae-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="219ae-111">**Điểm đến địa chỉ hoặc giá trị**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="219ae-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="219ae-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="219ae-112">**TTL**: 3600</span></span>

   <span data-ttu-id="219ae-113">\<DomainGUID\>là văn bản bên trái `.mail.protection.outlook.com` trong bản ghi MX tùy chỉnh cho miền tùy biến (ví dụ: `contoso-com` đối với miền contoso.com).</span><span class="sxs-lookup"><span data-stu-id="219ae-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="219ae-114">\<InitialDomain\>là tên miền bạn đã sử dụng khi đăng ký Microsoft 365 (ví dụ: contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="219ae-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="219ae-115">Sau khi bạn đã tạo bản ghi CNAME cho miền tùy chỉnh của mình, hãy hoàn tất các hướng dẫn sau:</span><span class="sxs-lookup"><span data-stu-id="219ae-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="219ae-116">A.</span><span class="sxs-lookup"><span data-stu-id="219ae-116">a.</span></span> <span data-ttu-id="219ae-117">[đăng nhập vào Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) bằng tài khoản nơi làm việc hoặc trường học của bạn.</span><span class="sxs-lookup"><span data-stu-id="219ae-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="219ae-118">B.</span><span class="sxs-lookup"><span data-stu-id="219ae-118">b.</span></span> <span data-ttu-id="219ae-119">Chọn biểu tượng trình khởi chạy ứng dụng ở góc trên bên trái và chọn **quản trị viên**.</span><span class="sxs-lookup"><span data-stu-id="219ae-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="219ae-120">C.</span><span class="sxs-lookup"><span data-stu-id="219ae-120">c.</span></span> <span data-ttu-id="219ae-121">Ở phía dưới bên trái điều hướng, mở rộng **quản trị** và chọn **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="219ae-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="219ae-122">D.</span><span class="sxs-lookup"><span data-stu-id="219ae-122">d.</span></span> <span data-ttu-id="219ae-123">Đi đến **bảo vệ**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="219ae-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="219ae-124">E.</span><span class="sxs-lookup"><span data-stu-id="219ae-124">e.</span></span> <span data-ttu-id="219ae-125">Chọn miền và sau đó chọn **bật** để **ký thư cho miền này bằng chữ ký DKIM**.</span><span class="sxs-lookup"><span data-stu-id="219ae-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="219ae-126">Lặp lại bước này cho mỗi miền tùy chỉnh.</span><span class="sxs-lookup"><span data-stu-id="219ae-126">Repeat this step for each custom domain.</span></span>
