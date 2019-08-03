---
title: Gỡ rối các vấn đề - không tìm thấy người dùng trong thư mục
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0909edc581c811fdc4683b004e0df0adbac88d1c
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35249935"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="22044-102">Gỡ rối các vấn đề - không tìm thấy người dùng trong thư mục</span><span class="sxs-lookup"><span data-stu-id="22044-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="22044-103">Nếu người dùng nhận được lỗi thông báo "không thể được tìm thấy người dùng" trong thư mục.</span><span class="sxs-lookup"><span data-stu-id="22044-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="22044-104">Hãy thử một lần nữa nơi loại vấn đề là người dùng không phải trong thư mục.</span><span class="sxs-lookup"><span data-stu-id="22044-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="22044-105">Các bước sau đây có thể được hoàn thành để khắc phục vấn đề.</span><span class="sxs-lookup"><span data-stu-id="22044-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="22044-106">Đảm bảo tài khoản có chấp nhận lời mời email cùng một tài khoản đang được sử dụng để đăng nhập sau.</span><span class="sxs-lookup"><span data-stu-id="22044-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="22044-107">Đảm bảo rằng người dùng đang sử dụng cùng một tài khoản để chấp nhận lời mời và đăng nhập vào trang web.</span><span class="sxs-lookup"><span data-stu-id="22044-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="22044-108">Để biết thêm thông tin, hãy xem [làm thế nào để quản lý các bí danh cho tài khoản Microsoft của bạn</a> để quản lý các đăng nhập Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="22044-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="22044-109">Trình duyệt cho mỗi trang web mà người dùng nhận được các lỗi.</span><span class="sxs-lookup"><span data-stu-id="22044-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="22044-110">Thêm "/ _layouts/15/people.aspx/membershipgroupid=0" (trong các kép, dấu ngoặc kép) vào cuối URL của trang web.</span><span class="sxs-lookup"><span data-stu-id="22044-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="22044-111">Ví dụ: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="22044-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="22044-112">Chọn người dùng từ danh sách.</span><span class="sxs-lookup"><span data-stu-id="22044-112">Select the user from the list.</span></span>

- <span data-ttu-id="22044-113">Nhấp vào **xoá người sử dụng quyền hạn** từ Ribbon.</span><span class="sxs-lookup"><span data-stu-id="22044-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="22044-114">Thêm về người dùng và gửi lại mời cho người dùng.</span><span class="sxs-lookup"><span data-stu-id="22044-114">Add back the User and Resend the invite to the user.</span></span>

