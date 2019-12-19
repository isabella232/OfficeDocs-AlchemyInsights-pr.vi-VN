---
title: Đã có lỗi xác nhận truy cập lỗi mã thông báo trong máy tính để bàn phân tích trên máy bay
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741310"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="ee245-102">"Đã có lỗi xác nhận truy cập mã thông báo" lỗi trong máy tính để bàn phân tích bộ nhớ ngoài</span><span class="sxs-lookup"><span data-stu-id="ee245-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="ee245-103">Lỗi này thường được quan sát khi mã thông báo xác thực hết hạn.</span><span class="sxs-lookup"><span data-stu-id="ee245-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="ee245-104">Thông thường, làm mới trang làm mới các mã thông báo.</span><span class="sxs-lookup"><span data-stu-id="ee245-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="ee245-105">Tuy nhiên, sự cố này có thể tồn tại nếu có bất kỳ chính sách truy cập có điều kiện áp dụng cho tài khoản được sử dụng trên máy tính để bàn phân tích.</span><span class="sxs-lookup"><span data-stu-id="ee245-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="ee245-106">Bạn có thể xem Nhật ký Azure AD đăng nhập trong cổng Azure để biết nếu có bất kỳ lỗi đăng nhập cho tài khoản đang được sử dụng cho máy tính để bàn phân tích onboarding.</span><span class="sxs-lookup"><span data-stu-id="ee245-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="ee245-107">Để biết thêm thông tin về truy nhập có điều kiện, truy cập [kế hoạch triển khai truy cập có điều kiện của bạn](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="ee245-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>