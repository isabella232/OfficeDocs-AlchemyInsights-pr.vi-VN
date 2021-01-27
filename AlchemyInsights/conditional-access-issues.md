---
title: Các vấn đề truy nhập có điều kiện
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015007"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="f68fb-102">Các vấn đề truy nhập có điều kiện</span><span class="sxs-lookup"><span data-stu-id="f68fb-102">Conditional access issues</span></span>

<span data-ttu-id="f68fb-103">**Giải quyết vấn đề khi chẩn đoán đăng nhập**</span><span class="sxs-lookup"><span data-stu-id="f68fb-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="f68fb-104">Bạn có thể nhanh chóng tìm hiểu điều gì đã xảy ra hoặc chẩn đoán các vấn đề liên quan đến người dùng đăng nhập bằng cách sử dụng [chẩn đoán đăng nhập](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="f68fb-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="f68fb-105">Khởi động chẩn đoán đăng nhập.</span><span class="sxs-lookup"><span data-stu-id="f68fb-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="f68fb-106">Tìm sự kiện để phân tích bằng cách nhập vào các chi tiết bạn có về người dùng, ứng dụng, thời gian đăng nhập, yêu cầu ID hoặc tương quan ID.</span><span class="sxs-lookup"><span data-stu-id="f68fb-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="f68fb-107">Xem lại kết quả chẩn đoán Hiển thị chi tiết về những điều đã xảy ra và những hành động bạn có thể thực hiện để thay đổi (nếu có bất kỳ thay đổi nào cần thiết).</span><span class="sxs-lookup"><span data-stu-id="f68fb-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="f68fb-108">**Các bước để khắc phục sự cố đăng nhập**</span><span class="sxs-lookup"><span data-stu-id="f68fb-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="f68fb-109">Dẫn hướng đến trang đăng nhập Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f68fb-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="f68fb-110">Lọc đăng nhập bằng người dùng, phạm vi thời gian, ứng dụng, trạng thái, ứng dụng khách, v.v.</span><span class="sxs-lookup"><span data-stu-id="f68fb-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="f68fb-111">Chọn sự kiện đăng nhập và xem tab truy nhập có điều kiện để xem các chính sách nào được đánh giá.</span><span class="sxs-lookup"><span data-stu-id="f68fb-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="f68fb-112">Bấm vào hàng của chính sách để xem chi tiết chính sách và hiểu tại sao nó được áp dụng.</span><span class="sxs-lookup"><span data-stu-id="f68fb-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="f68fb-113">**Công cụ để khắc phục sự cố chính sách truy nhập có điều kiện**</span><span class="sxs-lookup"><span data-stu-id="f68fb-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="f68fb-114">Chế độ chỉ báo cáo cho phép bạn đánh giá chính sách mà không tác động đến người dùng.</span><span class="sxs-lookup"><span data-stu-id="f68fb-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="f68fb-115">Công cụ điều gì sẽ cho phép bạn mô phỏng các sự kiện đăng nhập và xem các chính sách nào sẽ áp dụng.</span><span class="sxs-lookup"><span data-stu-id="f68fb-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="f68fb-116">Sổ làm việc hiểu biết và báo cáo hiển thị ảnh hưởng theo thời gian thực của mỗi chính sách.</span><span class="sxs-lookup"><span data-stu-id="f68fb-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="f68fb-117">**Chính sách bảo vệ đường cơ sở**</span><span class="sxs-lookup"><span data-stu-id="f68fb-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="f68fb-118">Các chính sách bảo vệ đường cơ sở đã bị suy giảm.</span><span class="sxs-lookup"><span data-stu-id="f68fb-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="f68fb-119">Chúng không còn được áp thi và sẽ sớm được loại bỏ khỏi Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="f68fb-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="f68fb-120">Chúng tôi khuyên bạn nên bật tính năng [mặc định bảo mật](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="f68fb-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="f68fb-121">Để biết thêm thông tin về truy nhập có điều kiện, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="f68fb-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="f68fb-122">Các cách [thực hành tốt nhất để truy nhập có điều kiện trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 Các [điều kiện trong quyền truy nhập](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 có điều kiện [Điều khiển trong quyền truy nhập](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 có điều kiện [Vị trí trong Access](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition) có điều kiện</span><span class="sxs-lookup"><span data-stu-id="f68fb-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
