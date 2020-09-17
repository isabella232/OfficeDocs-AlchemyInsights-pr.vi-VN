---
title: Đã xảy ra lỗi khi xác nhận lỗi mã truy nhập trong khi phân tích máy tính tại chỗ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783573"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="c13ba-102">Lỗi "đã xảy ra lỗi khi xác nhận mã truy nhập" trong khi phân tích máy tính để bàn triển khai</span><span class="sxs-lookup"><span data-stu-id="c13ba-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="c13ba-103">Lỗi này thường được quan sát thấy khi mã xác thực hết hạn.</span><span class="sxs-lookup"><span data-stu-id="c13ba-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="c13ba-104">Thông thường, làm mới trang sẽ làm mới mã thông báo.</span><span class="sxs-lookup"><span data-stu-id="c13ba-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="c13ba-105">Tuy nhiên, sự cố này có thể tồn tại nếu có bất kỳ chính sách truy nhập có điều kiện nào được áp dụng cho tài khoản đang được sử dụng để phân tích trên máy tính bảng.</span><span class="sxs-lookup"><span data-stu-id="c13ba-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="c13ba-106">Bạn có thể xem lại đăng nhập Azure AD trong các Nhật ký trong cổng thông tin Azure để xem liệu có bất kỳ lỗi đăng nhập nào cho tài khoản đang được sử dụng cho máy tính để bàn onboarding không.</span><span class="sxs-lookup"><span data-stu-id="c13ba-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="c13ba-107">Để biết thêm thông tin về truy nhập có điều kiện, hãy truy cập [lên kế hoạch triển khai truy nhập](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)có điều kiện.</span><span class="sxs-lookup"><span data-stu-id="c13ba-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>