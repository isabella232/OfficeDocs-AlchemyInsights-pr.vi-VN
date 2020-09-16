---
title: Khắc phục sự cố-người dùng không tìm thấy trong thư mục
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725429"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="eaf9b-102">Khắc phục sự cố-người dùng không tìm thấy trong thư mục</span><span class="sxs-lookup"><span data-stu-id="eaf9b-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="eaf9b-103">Nếu người dùng đang nhận được thông báo lỗi "không thể tìm thấy người dùng" trong thư mục, vui lòng thử lại nơi mà kiểu vấn đề là người dùng không có trong thư mục.</span><span class="sxs-lookup"><span data-stu-id="eaf9b-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="eaf9b-104">Các bước sau đây có thể được hoàn tất để khắc phục sự cố này.</span><span class="sxs-lookup"><span data-stu-id="eaf9b-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="eaf9b-105">Đảm bảo tài khoản chấp nhận lời mời email là cùng một tài khoản đang được sử dụng để đăng nhập sau đó.</span><span class="sxs-lookup"><span data-stu-id="eaf9b-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="eaf9b-106">Đảm bảo rằng người dùng đang sử dụng cùng một tài khoản để chấp nhận lời mời và đăng nhập vào trang.</span><span class="sxs-lookup"><span data-stu-id="eaf9b-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="eaf9b-107">Để biết thêm thông tin, hãy xem [cách quản lý biệt danh cho tài khoản Microsoft của bạn </a> để quản lý đăng nhập Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="eaf9b-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="eaf9b-108">Duyệt đến từng (các) site mà người dùng đang nhận được lỗi.</span><span class="sxs-lookup"><span data-stu-id="eaf9b-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="eaf9b-109">Thêm "/_layouts/15/17/người. aspx/membershipgroupid = 0" (trong dấu ngoặc kép) đến cuối URL của site.</span><span class="sxs-lookup"><span data-stu-id="eaf9b-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="eaf9b-110">Ví dụ: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="eaf9b-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="eaf9b-111">Chọn người dùng từ danh sách.</span><span class="sxs-lookup"><span data-stu-id="eaf9b-111">Select the user from the list.</span></span>

- <span data-ttu-id="eaf9b-112">Bấm **loại bỏ quyền của người dùng** khỏi dải băng.</span><span class="sxs-lookup"><span data-stu-id="eaf9b-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="eaf9b-113">Thêm lại người dùng và gửi lại lời mời cho người dùng.</span><span class="sxs-lookup"><span data-stu-id="eaf9b-113">Add back the User and Resend the invite to the user.</span></span>

