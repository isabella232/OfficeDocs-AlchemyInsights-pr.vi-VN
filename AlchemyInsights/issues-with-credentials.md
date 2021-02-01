---
title: Các vấn đề với chứng danh
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063724"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="97496-102">Các vấn đề với chứng danh</span><span class="sxs-lookup"><span data-stu-id="97496-102">Issues with credentials</span></span>

<span data-ttu-id="97496-103">[Nền tảng Microsoft Identity và dòng chứng danh máy khách oauth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) mô tả cách chương trình trực tiếp chống lại chứng danh máy khách của oauth 2,0.</span><span class="sxs-lookup"><span data-stu-id="97496-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="97496-104">**Làm thế nào để tôi quản lý mật khẩu của ứng dụng hoặc chứng danh chứng chỉ?**</span><span class="sxs-lookup"><span data-stu-id="97496-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="97496-105">Trong Azure CLI, bạn có thể sử dụng thông tin xác thực [ứng dụng AZ AD](https://docs.microsoft.com/cli/azure/ad/app/credential) để xóa, danh sách hoặc đặt lại mật khẩu hoặc chứng danh chứng chỉ của ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="97496-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="97496-106">**Làm thế nào để người dùng của tôi đặt lại mật khẩu?**</span><span class="sxs-lookup"><span data-stu-id="97496-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="97496-107">Người dùng cần [đăng ký để đặt lại mật khẩu tự phục vụ](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) trước khi họ có thể đặt lại mật khẩu của họ.</span><span class="sxs-lookup"><span data-stu-id="97496-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="97496-108">Sau khi người dùng đã đăng ký, họ có thể làm theo các hướng dẫn trong bài viết này để đặt lại mật khẩu của họ: [đặt lại mật khẩu cơ quan hoặc trường học của bạn](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span><span class="sxs-lookup"><span data-stu-id="97496-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="97496-109">**Người dùng của tôi thay đổi mật khẩu của mình như thế nào?**</span><span class="sxs-lookup"><span data-stu-id="97496-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="97496-110">Người dùng có thể làm theo các bước trong bài viết này để thay đổi mật khẩu của họ: [cách thay đổi mật khẩu của bạn](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span><span class="sxs-lookup"><span data-stu-id="97496-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="97496-111">Họ cũng có thể [quản lý mật khẩu ứng dụng để xác minh hai bước](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span><span class="sxs-lookup"><span data-stu-id="97496-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="97496-112">**Người dùng của tôi đang nhận được lỗi khi thay đổi hoặc đặt lại mật khẩu của họ**</span><span class="sxs-lookup"><span data-stu-id="97496-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="97496-113">Liên kết này sẽ cung cấp thông tin về các sự cố phổ biến có thể phát sinh khi người dùng đang tìm cách đặt lại mật khẩu: các [vấn đề thường gặp và giải pháp của họ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="97496-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="97496-114">**Tôi đang gặp sự cố khi đặt lại mật khẩu của người dùng**</span><span class="sxs-lookup"><span data-stu-id="97496-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="97496-115">Hãy đảm bảo rằng bạn được ủy quyền để đặt lại mật khẩu.</span><span class="sxs-lookup"><span data-stu-id="97496-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="97496-116">*Chỉ có người quản trị toàn cầu, mật khẩu và người dùng có thể đặt lại mật khẩu người dùng.*</span><span class="sxs-lookup"><span data-stu-id="97496-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="97496-117">Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị đặc quyền khác.</span><span class="sxs-lookup"><span data-stu-id="97496-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="97496-118">Hãy đảm bảo bạn hiểu được các yêu cầu cấp phép:</span><span class="sxs-lookup"><span data-stu-id="97496-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="97496-119">Bạn phải có ít nhất một giấy phép được gán trong tổ chức của bạn:</span><span class="sxs-lookup"><span data-stu-id="97496-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="97496-120">**Đám mây chỉ người dùng** -bất kỳ Office 365 (O365) được trả về SKU hoặc Azure AD BASIC</span><span class="sxs-lookup"><span data-stu-id="97496-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="97496-121">Nền tảng điện **toán đám mây và/hoặc người dùng tại cơ sở** -Azure AD Premium P1 hoặc P2, doanh nghiệp Mobility + Security (EMS), hoặc doanh nghiệp hiệu quả bảo mật (SPE)</span><span class="sxs-lookup"><span data-stu-id="97496-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="97496-122">Để tìm hiểu thêm về các yêu cầu cấp phép, hãy xem các [yêu cầu cấp phép cho AZURE AD tự đặt lại mật khẩu](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span><span class="sxs-lookup"><span data-stu-id="97496-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="97496-123">Để đặt lại mật khẩu người dùng, hãy tìm người dùng trong Azure AD.</span><span class="sxs-lookup"><span data-stu-id="97496-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="97496-124">Sau đó, trên lưỡi tổng quan cho người dùng đó, hãy bấm vào nút "đặt lại mật khẩu".</span><span class="sxs-lookup"><span data-stu-id="97496-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="97496-125">**Nút đặt lại mật khẩu bị mờ đi**</span><span class="sxs-lookup"><span data-stu-id="97496-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="97496-126">Bạn không được phép đặt lại mật khẩu của người dùng **này** .</span><span class="sxs-lookup"><span data-stu-id="97496-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="97496-127">*Chỉ có người quản trị toàn cầu, mật khẩu và người dùng có thể đặt lại mật khẩu người dùng.*</span><span class="sxs-lookup"><span data-stu-id="97496-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="97496-128">Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị đặc quyền khác.</span><span class="sxs-lookup"><span data-stu-id="97496-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="97496-129">**Tôi không nhìn thấy lưỡi đặt lại mật khẩu**</span><span class="sxs-lookup"><span data-stu-id="97496-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="97496-130">Bạn không được phép đặt lại mật khẩu.</span><span class="sxs-lookup"><span data-stu-id="97496-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="97496-131">*Chỉ có người quản trị toàn cầu, mật khẩu và người dùng có thể đặt lại mật khẩu người dùng.*</span><span class="sxs-lookup"><span data-stu-id="97496-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="97496-132">Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị đặc quyền khác.</span><span class="sxs-lookup"><span data-stu-id="97496-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="97496-133">**Tôi không nhìn thấy lưỡi kiếm tích hợp tại cơ sở trong đặt lại mật khẩu**</span><span class="sxs-lookup"><span data-stu-id="97496-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="97496-134">Lưỡi tích hợp tại cơ sở chỉ xuất hiện trong môi trường hỗn hợp-nghĩa là bạn đang sử dụng writeback để thao tác mật khẩu của người dùng tại cơ sở.</span><span class="sxs-lookup"><span data-stu-id="97496-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="97496-135">Bạn không thấy lưỡi này nếu:</span><span class="sxs-lookup"><span data-stu-id="97496-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="97496-136">Bạn không sử dụng writeback mật khẩu</span><span class="sxs-lookup"><span data-stu-id="97496-136">You are not using password writeback</span></span>
  - <span data-ttu-id="97496-137">Có vấn đề với việc cài đặt/kết nối của writeback mật khẩu</span><span class="sxs-lookup"><span data-stu-id="97496-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="97496-138">Có vấn đề với việc cài đặt/kết nối của Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="97496-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="97496-139">Để biết thêm các bước khắc phục sự cố với mật khẩu trở lại, hãy xem [khắc phục sự cố writeback mật khẩu](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="97496-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="97496-140">**Tôi không biết làm thế nào để đặt lại mật khẩu người dùng**</span><span class="sxs-lookup"><span data-stu-id="97496-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="97496-141">Đăng nhập vào cổng thông tin Azure với tư cách là người quản trị thích hợp.</span><span class="sxs-lookup"><span data-stu-id="97496-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="97496-142">Đi đến lưỡi **người dùng và nhóm** , chọn **tất cả người dùng**.</span><span class="sxs-lookup"><span data-stu-id="97496-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="97496-143">Chọn một người dùng từ danh sách.</span><span class="sxs-lookup"><span data-stu-id="97496-143">Select a user from the list.</span></span>
4. <span data-ttu-id="97496-144">Đối với người dùng đã chọn, hãy chọn **tổng quan**, rồi trong thanh lệnh, chọn **đặt lại mật khẩu**.</span><span class="sxs-lookup"><span data-stu-id="97496-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="97496-145">Chọn nút **đặt lại mật khẩu** và làm theo hướng dẫn trên màn hình.</span><span class="sxs-lookup"><span data-stu-id="97496-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="97496-146">Chỉ Reset được thực hiện thông qua dịch vụ hỗ trợ **Azure Portal** .</span><span class="sxs-lookup"><span data-stu-id="97496-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="97496-147">**Tôi đặt lại mật khẩu người dùng tại cơ sở từ cổng thông tin quản trị Office 365 hoặc ứng dụng Office 365 dành cho thiết bị di động nhưng người dùng vẫn không thể đăng nhập**</span><span class="sxs-lookup"><span data-stu-id="97496-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="97496-148">Không hỗ trợ mật khẩu của Writeback trong cổng thông tin này.</span><span class="sxs-lookup"><span data-stu-id="97496-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="97496-149">Đặt lại mật khẩu người dùng một lần nữa trong cổng thông tin Azure.</span><span class="sxs-lookup"><span data-stu-id="97496-149">Reset the user's password again in the Azure portal.</span></span>
