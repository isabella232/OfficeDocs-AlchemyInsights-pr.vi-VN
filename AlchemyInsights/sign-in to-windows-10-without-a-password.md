---
title: Đăng nhập vào Windows 10 mà không cần dùng mật khẩu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830568"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="cd3da-102">Đăng nhập vào Windows 10 mà không cần dùng mật khẩu</span><span class="sxs-lookup"><span data-stu-id="cd3da-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="cd3da-103">Để tránh việc nhập mật khẩu tại khởi động Windows, chúng tôi khuyên bạn nên sử dụng một trong các tùy chọn đăng nhập bảo mật của Windows hello, chẳng hạn như mã PIN, nhận diện khuôn mặt hoặc dấu vân tay, nếu có.</span><span class="sxs-lookup"><span data-stu-id="cd3da-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="cd3da-104">Nếu bạn thực sự muốn tắt tính năng đăng nhập bảo mật, hãy xem hướng dẫn "tự động đăng nhập vào Windows 10" bên dưới.</span><span class="sxs-lookup"><span data-stu-id="cd3da-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="cd3da-105">**Bảo mật cho các lựa chọn thay thế Windows hello vào mật khẩu tài khoản**</span><span class="sxs-lookup"><span data-stu-id="cd3da-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="cd3da-106">Đi đến **cài đặt > tài khoản > các tùy chọn đăng nhập** (hoặc bấm vào [đây](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="cd3da-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="cd3da-107">Các tùy chọn đăng nhập sẵn dùng sẽ được liệt kê.</span><span class="sxs-lookup"><span data-stu-id="cd3da-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="cd3da-108">Ví dụ:</span><span class="sxs-lookup"><span data-stu-id="cd3da-108">For example:</span></span>

![Các tùy chọn đăng nhập.](media/sign-in-options.png)

<span data-ttu-id="cd3da-110">Bấm hoặc gõ nhẹ vào một trong các tùy chọn để cấu hình.</span><span class="sxs-lookup"><span data-stu-id="cd3da-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="cd3da-111">Lần sau khi bạn khởi động hoặc mở khóa Windows, bạn sẽ có thể sử dụng tùy chọn mới thay vì mật khẩu.</span><span class="sxs-lookup"><span data-stu-id="cd3da-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="cd3da-112">**Đăng nhập tự động vào Windows 10**</span><span class="sxs-lookup"><span data-stu-id="cd3da-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="cd3da-113">**Lưu ý**: việc đăng nhập tự động thuận tiện, nhưng giới thiệu một rủi ro bảo mật, đặc biệt là nếu PC của bạn có thể truy nhập được nhiều người.</span><span class="sxs-lookup"><span data-stu-id="cd3da-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="cd3da-114">Bấm hoặc gõ nhẹ vào nút **bắt đầu** trong thanh tác vụ.</span><span class="sxs-lookup"><span data-stu-id="cd3da-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="cd3da-115">Nhập **netplwiz** và nhấn phím Enter để mở cửa sổ tài khoản người dùng.</span><span class="sxs-lookup"><span data-stu-id="cd3da-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="cd3da-116">Trong **tài khoản người dùng**, hãy bấm vào tài khoản mà bạn muốn tự động đăng nhập vào khi Windows khởi động.</span><span class="sxs-lookup"><span data-stu-id="cd3da-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="cd3da-117">Bỏ chọn hộp kiểm "người dùng phải nhập tên người dùng và mật khẩu để dùng hộp kiểm" máy tính này.</span><span class="sxs-lookup"><span data-stu-id="cd3da-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Người dùng phải nhập tùy chọn tên người dùng và mật khẩu.](media/users-must-enter-username.png)

5. <span data-ttu-id="cd3da-119">Bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="cd3da-119">Click **OK**.</span></span> <span data-ttu-id="cd3da-120">Bạn sẽ được yêu cầu nhập và xác nhận mật khẩu cho tài khoản mà bạn đã chọn.</span><span class="sxs-lookup"><span data-stu-id="cd3da-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="cd3da-121">Bấm vào **OK** để kết thúc.</span><span class="sxs-lookup"><span data-stu-id="cd3da-121">Click **OK** to finish.</span></span> <span data-ttu-id="cd3da-122">Thời gian tiếp theo, Windows 10 bắt đầu, nó sẽ tự động đăng nhập vào tài khoản mà bạn đã chọn.</span><span class="sxs-lookup"><span data-stu-id="cd3da-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
