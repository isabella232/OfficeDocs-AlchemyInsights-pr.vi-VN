---
title: Thiết lập TKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808729"
---
# <a name="setup-dkim"></a><span data-ttu-id="e546c-102">Thiết lập TKIM</span><span class="sxs-lookup"><span data-stu-id="e546c-102">Setup DKIM</span></span>

<span data-ttu-id="e546c-103">Hướng dẫn đầy đủ để đặt cấu hình cho các tên miền tùy chỉnh trong Microsoft 365 ở [đây](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="e546c-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="e546c-104">Đối với **mỗi** tên miền tùy chỉnh, bạn cần phải tạo **hai** bản ghi CNAME trên máy chủ lưu trữ DNS của tên miền của bạn (thường là cơ quan đăng ký tên miền).</span><span class="sxs-lookup"><span data-stu-id="e546c-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="e546c-105">Ví dụ, contoso.com và fourthcoffee.com yêu cầu bốn bản ghi CNAME được tạo: hai cho contoso.com và hai đối với fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="e546c-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="e546c-106">Bản ghi CNAME của **MKIM cho mỗi** tên miền tùy chỉnh sử dụng các định dạng sau:</span><span class="sxs-lookup"><span data-stu-id="e546c-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="e546c-107">**Tên máy chủ**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="e546c-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="e546c-108">**Trỏ tới địa chỉ hoặc giá trị**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="e546c-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="e546c-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="e546c-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="e546c-110">**Tên máy chủ**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="e546c-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="e546c-111">**Trỏ tới địa chỉ hoặc giá trị**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="e546c-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="e546c-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="e546c-112">**TTL**: 3600</span></span>

   <span data-ttu-id="e546c-113">\<DomainGUID\> là văn bản ở bên trái `.mail.protection.outlook.com` trong bản ghi MX tùy chỉnh cho tên miền tùy chỉnh (ví dụ: `contoso-com` đối với tên miền contoso.com).</span><span class="sxs-lookup"><span data-stu-id="e546c-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="e546c-114">\<InitialDomain\> là tên miền mà bạn đã sử dụng khi đăng ký Microsoft 365 (ví dụ, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="e546c-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="e546c-115">Sau khi bạn đã tạo bản ghi CNAME cho tên miền riêng của mình, hãy hoàn thành các hướng dẫn sau đây:</span><span class="sxs-lookup"><span data-stu-id="e546c-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="e546c-116">một.</span><span class="sxs-lookup"><span data-stu-id="e546c-116">a.</span></span> <span data-ttu-id="e546c-117">[đăng nhập vào Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) bằng tài khoản cơ quan hoặc trường học của bạn.</span><span class="sxs-lookup"><span data-stu-id="e546c-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="e546c-118">b.</span><span class="sxs-lookup"><span data-stu-id="e546c-118">b.</span></span> <span data-ttu-id="e546c-119">Chọn biểu tượng công cụ khởi động ứng dụng ở phía trên bên trái, rồi chọn người **quản trị**.</span><span class="sxs-lookup"><span data-stu-id="e546c-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="e546c-120">c's.</span><span class="sxs-lookup"><span data-stu-id="e546c-120">c.</span></span> <span data-ttu-id="e546c-121">Trong dẫn hướng phía dưới bên trái, hãy bung rộng **quản trị** và chọn **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="e546c-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="e546c-122">dâm.</span><span class="sxs-lookup"><span data-stu-id="e546c-122">d.</span></span> <span data-ttu-id="e546c-123">Đi đến **bảo vệ**  >  **d**.</span><span class="sxs-lookup"><span data-stu-id="e546c-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="e546c-124">e's.</span><span class="sxs-lookup"><span data-stu-id="e546c-124">e.</span></span> <span data-ttu-id="e546c-125">Chọn tên miền và sau đó chọn **bật** cho **tin nhắn đăng nhập cho tên miền này với chữ ký**trong dấu kim.</span><span class="sxs-lookup"><span data-stu-id="e546c-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="e546c-126">Lặp lại bước này cho mỗi tên miền tùy chỉnh.</span><span class="sxs-lookup"><span data-stu-id="e546c-126">Repeat this step for each custom domain.</span></span>
