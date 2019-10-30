---
title: Khắc phục sự cố-người dùng không tìm thấy trong thư mục
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768823"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="6686d-102">Khắc phục sự cố-người dùng không tìm thấy trong thư mục</span><span class="sxs-lookup"><span data-stu-id="6686d-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="6686d-103">Nếu người dùng nhận được thông báo lỗi "không thể tìm thấy người dùng" trong thư mục, vui lòng thử lại nơi loại sự cố là người dùng không có trong thư mục.</span><span class="sxs-lookup"><span data-stu-id="6686d-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="6686d-104">Các bước sau đây có thể được hoàn tất để khắc phục sự cố.</span><span class="sxs-lookup"><span data-stu-id="6686d-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="6686d-105">Đảm bảo tài khoản chấp nhận lời mời email là cùng một tài khoản đang được sử dụng để đăng nhập sau này.</span><span class="sxs-lookup"><span data-stu-id="6686d-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="6686d-106">Đảm bảo rằng người dùng đang sử dụng cùng một tài khoản để chấp nhận lời mời và đăng nhập vào trang web.</span><span class="sxs-lookup"><span data-stu-id="6686d-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="6686d-107">Để biết thêm thông tin, hãy xem [cách quản lý bí danh</a> cho tài khoản Microsoft của bạn để quản lý văn phòng 365 đăng nhập](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="6686d-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="6686d-108">Duyệt tới mỗi (các) trang web mà người dùng nhận được lỗi.</span><span class="sxs-lookup"><span data-stu-id="6686d-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="6686d-109">Thêm "/_layouts/15/nhân .aspx/membershipgroupid = 0" (trong các dấu ngoặc kép) đến cuối URL trang web.</span><span class="sxs-lookup"><span data-stu-id="6686d-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="6686d-110">Ví dụ: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="6686d-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="6686d-111">Chọn người dùng từ danh sách.</span><span class="sxs-lookup"><span data-stu-id="6686d-111">Select the user from the list.</span></span>

- <span data-ttu-id="6686d-112">Bấm **loại bỏ quyền của người dùng** từ ruy băng.</span><span class="sxs-lookup"><span data-stu-id="6686d-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="6686d-113">Thêm lùi người dùng và gửi lại lời mời cho người dùng.</span><span class="sxs-lookup"><span data-stu-id="6686d-113">Add back the User and Resend the invite to the user.</span></span>

