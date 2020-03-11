---
title: Đăng nhập vào Windows 10 mà không sử dụng mật khẩu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588302"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="abf1b-102">Đăng nhập vào Windows 10 mà không sử dụng mật khẩu</span><span class="sxs-lookup"><span data-stu-id="abf1b-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="abf1b-103">Để tránh phải nhập mật khẩu khi khởi động Windows, chúng tôi khuyên bạn nên sử dụng một trong các tùy chọn đăng nhập an toàn của Windows hello, như mã PIN, nhận dạng khuôn mặt hoặc dấu vân tay, nếu có.</span><span class="sxs-lookup"><span data-stu-id="abf1b-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="abf1b-104">Nếu bạn thực sự muốn vô hiệu hóa đăng nhập an toàn, hãy xem hướng dẫn "tự động đăng nhập vào Windows 10" bên dưới.</span><span class="sxs-lookup"><span data-stu-id="abf1b-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="abf1b-105">**Bảo mật Windows Hello thay thế cho mật khẩu tài khoản**</span><span class="sxs-lookup"><span data-stu-id="abf1b-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="abf1b-106">Đi tới **cài đặt > tài khoản > tùy chọn đăng nhập** (hoặc bấm vào [đây](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="abf1b-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="abf1b-107">Các tùy chọn đăng nhập có sẵn sẽ được liệt kê.</span><span class="sxs-lookup"><span data-stu-id="abf1b-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="abf1b-108">Ví dụ:</span><span class="sxs-lookup"><span data-stu-id="abf1b-108">For example:</span></span>

![Tùy chọn đăng nhập.](media/sign-in-options.png)

<span data-ttu-id="abf1b-110">Nhấp hoặc nhấn vào một trong các tùy chọn để cấu hình nó.</span><span class="sxs-lookup"><span data-stu-id="abf1b-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="abf1b-111">Lần tới khi bạn bắt đầu hoặc mở khóa Windows, bạn sẽ có thể sử dụng tùy chọn mới thay vì mật khẩu.</span><span class="sxs-lookup"><span data-stu-id="abf1b-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="abf1b-112">**Tự động đăng nhập vào Windows 10**</span><span class="sxs-lookup"><span data-stu-id="abf1b-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="abf1b-113">**Lưu ý**: đăng nhập tự động là thuận tiện, nhưng giới thiệu một rủi ro bảo mật, đặc biệt là nếu máy tính của bạn có thể truy cập bởi nhiều người.</span><span class="sxs-lookup"><span data-stu-id="abf1b-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="abf1b-114">Nhấp hoặc nhấn vào nút **bắt đầu** trong thanh tác vụ.</span><span class="sxs-lookup"><span data-stu-id="abf1b-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="abf1b-115">Nhập **netplwiz** và nhấn phím Enter để mở cửa sổ tài khoản người dùng.</span><span class="sxs-lookup"><span data-stu-id="abf1b-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="abf1b-116">Trong **tài khoản người dùng**, bấm vào tài khoản mà bạn muốn tự động đăng nhập khi Windows bắt đầu.</span><span class="sxs-lookup"><span data-stu-id="abf1b-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="abf1b-117">Bỏ chọn hộp kiểm "người dùng phải nhập tên người dùng và mật khẩu để sử dụng máy tính này".</span><span class="sxs-lookup"><span data-stu-id="abf1b-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Người dùng phải nhập tùy chọn tên người dùng và mật khẩu.](media/users-must-enter-username.png)

5. <span data-ttu-id="abf1b-119">Bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="abf1b-119">Click **OK**.</span></span> <span data-ttu-id="abf1b-120">Bạn sẽ được yêu cầu nhập và xác nhận mật khẩu cho tài khoản bạn đã chọn.</span><span class="sxs-lookup"><span data-stu-id="abf1b-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="abf1b-121">Nhấp vào **OK** để kết thúc.</span><span class="sxs-lookup"><span data-stu-id="abf1b-121">Click **OK** to finish.</span></span> <span data-ttu-id="abf1b-122">Lần tiếp theo, Windows 10 bắt đầu, nó sẽ tự động đăng nhập vào tài khoản bạn đã chọn.</span><span class="sxs-lookup"><span data-stu-id="abf1b-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
