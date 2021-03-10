---
title: Vấn đề đặt lại mật khẩu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696283"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="11939-102">Các vấn đề về việc đặt lại mật khẩu</span><span class="sxs-lookup"><span data-stu-id="11939-102">Problems resetting password</span></span>

<span data-ttu-id="11939-103">Sau đây là một số vấn đề mà bạn có thể gặp phải khi đặt lại mật khẩu và các giải pháp có thể xảy ra:</span><span class="sxs-lookup"><span data-stu-id="11939-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="11939-104">**Tôi đang gặp vấn đề với việc đặt lại mật khẩu không được bảo vệ trong các thể loại khác**</span><span class="sxs-lookup"><span data-stu-id="11939-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="11939-105">Đảm bảo bạn được ủy quyền để đặt lại mật khẩu.</span><span class="sxs-lookup"><span data-stu-id="11939-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="11939-106">Chỉ có người quản trị toàn cầu, mật khẩu và người dùng có thể đặt lại mật khẩu người dùng.</span><span class="sxs-lookup"><span data-stu-id="11939-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="11939-107">Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị đặc quyền khác.</span><span class="sxs-lookup"><span data-stu-id="11939-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="11939-108">Đảm bảo rằng bạn hiểu được các yêu cầu cấp phép:</span><span class="sxs-lookup"><span data-stu-id="11939-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="11939-109">Bạn phải có ít nhất một giấy phép được gán trong tổ chức của bạn</span><span class="sxs-lookup"><span data-stu-id="11939-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="11939-110">Đám mây chỉ người dùng-bất kỳ Office 365 (O365) được trả về SKU hoặc Azure AD BASIC</span><span class="sxs-lookup"><span data-stu-id="11939-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="11939-111">Nền tảng điện toán đám mây và/hoặc người dùng tại cơ sở-Azure AD Premium P1 hoặc P2, doanh nghiệp Mobility + Security (EMS), hoặc doanh nghiệp hiệu quả bảo mật (SPE)</span><span class="sxs-lookup"><span data-stu-id="11939-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="11939-112">Để đọc thêm về các yêu cầu cấp phép, hãy xem bài viết các [yêu cầu cấp phép cho AZURE AD tự đặt lại mật khẩu](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="11939-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="11939-113">**Tôi đang gặp vấn đề khi kiểm tra chính sách đặt lại mật khẩu tôi đặt**</span><span class="sxs-lookup"><span data-stu-id="11939-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="11939-114">Các chính sách được áp dụng gần đây có thể mất vài phút để sao chép trên tất cả các trung tâm dữ liệu và điểm cuối.</span><span class="sxs-lookup"><span data-stu-id="11939-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="11939-115">Khoảng cách vật lý từ Trung tâm dữ liệu cũng sẽ ảnh hưởng đến cách áp dụng các thay đổi nhanh chóng.</span><span class="sxs-lookup"><span data-stu-id="11939-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="11939-116">Kiểm tra với người dùng cuối, chứ không phải là người quản trị và thí điểm có một tập hợp người dùng nhỏ.</span><span class="sxs-lookup"><span data-stu-id="11939-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="11939-117">Các chính sách được cấu hình trong cổng thông tin Azure chỉ áp dụng cho người dùng cuối, chứ không phải người quản trị.</span><span class="sxs-lookup"><span data-stu-id="11939-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="11939-118">Microsoft hỗ trợ một chính sách đặt lại mật khẩu hai cổng mặc định mạnh cho bất kỳ vai trò người quản trị Azure nào (ví dụ: người quản trị toàn cầu, người quản trị, người quản trị mật khẩu, v.v.)</span><span class="sxs-lookup"><span data-stu-id="11939-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="11939-119">Tìm hiểu thêm về [chính sách dành cho người quản trị](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="11939-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="11939-120">**Tôi muốn triển khai đặt lại mật khẩu nhưng không muốn người dùng của tôi đăng ký thông tin bảo mật bổ sung**</span><span class="sxs-lookup"><span data-stu-id="11939-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="11939-121">Dữ liệu trước khi cư trú cho người dùng của bạn để họ không có!</span><span class="sxs-lookup"><span data-stu-id="11939-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="11939-122">-Với tư cách là người quản trị, bạn có thể đặt các thuộc tính điện thoại và email cho người dùng của bạn trước khi đặt lại mật khẩu cho tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="11939-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="11939-123">Bạn có thể thực hiện điều này bằng cách dùng API, PowerShell hoặc Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="11939-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="11939-124">Xem thêm thông tin tại đây:</span><span class="sxs-lookup"><span data-stu-id="11939-124">More information here:</span></span>
- [<span data-ttu-id="11939-125">Triển khai việc đặt lại mật khẩu mà không yêu cầu người dùng đăng ký</span><span class="sxs-lookup"><span data-stu-id="11939-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="11939-126">Việc đặt lại mật khẩu, dữ liệu nào được sử dụng</span><span class="sxs-lookup"><span data-stu-id="11939-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="11939-127">**Nút đặt lại mật khẩu bị mờ đi**</span><span class="sxs-lookup"><span data-stu-id="11939-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="11939-128">Bạn không được phép đặt lại mật khẩu của người dùng này.</span><span class="sxs-lookup"><span data-stu-id="11939-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="11939-129">Chỉ có người quản trị toàn cầu, mật khẩu và người dùng có thể đặt lại mật khẩu người dùng.</span><span class="sxs-lookup"><span data-stu-id="11939-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="11939-130">Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị đặc quyền khác.</span><span class="sxs-lookup"><span data-stu-id="11939-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="11939-131">**Tôi không nhìn thấy lưỡi đặt lại mật khẩu**</span><span class="sxs-lookup"><span data-stu-id="11939-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="11939-132">Bạn không được phép đặt lại mật khẩu.</span><span class="sxs-lookup"><span data-stu-id="11939-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="11939-133">Chỉ có người quản trị toàn cầu, mật khẩu và người dùng có thể đặt lại mật khẩu người dùng.</span><span class="sxs-lookup"><span data-stu-id="11939-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="11939-134">Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị đặc quyền khác.</span><span class="sxs-lookup"><span data-stu-id="11939-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="11939-135">**Tôi không nhìn thấy lưỡi kiếm tích hợp tại cơ sở trong đặt lại mật khẩu**</span><span class="sxs-lookup"><span data-stu-id="11939-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="11939-136">Lưỡi tích hợp tại cơ sở chỉ xuất hiện trong môi trường hỗn hợp-nghĩa là bạn đang sử dụng writeback để thao tác mật khẩu của người dùng tại cơ sở.</span><span class="sxs-lookup"><span data-stu-id="11939-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="11939-137">Bạn không thấy lưỡi này nếu:</span><span class="sxs-lookup"><span data-stu-id="11939-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="11939-138">Bạn không sử dụng writeback mật khẩu</span><span class="sxs-lookup"><span data-stu-id="11939-138">You are not using password writeback</span></span>
    - <span data-ttu-id="11939-139">Có vấn đề với việc cài đặt/kết nối của writeback mật khẩu</span><span class="sxs-lookup"><span data-stu-id="11939-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="11939-140">Có vấn đề với việc cài đặt/kết nối của Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="11939-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="11939-141">Để biết thêm các bước khắc phục sự cố với mật khẩu trở lại, hãy xem mục [khắc phục sự cố về mật khẩu](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="11939-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="11939-142">**Tôi không biết làm thế nào để đặt lại mật khẩu người dùng**</span><span class="sxs-lookup"><span data-stu-id="11939-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="11939-143">Đăng nhập vào cổng thông tin Azure với tư cách là người quản trị thích hợp.</span><span class="sxs-lookup"><span data-stu-id="11939-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="11939-144">Đi đến lưỡi người dùng và nhóm, chọn **tất cả người dùng**.</span><span class="sxs-lookup"><span data-stu-id="11939-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="11939-145">Chọn một người dùng từ danh sách.</span><span class="sxs-lookup"><span data-stu-id="11939-145">Select a user from the list.</span></span>
1. <span data-ttu-id="11939-146">Đối với người dùng đã chọn, hãy chọn **tổng quan**, sau đó trong thanh lệnh, hãy bấm **đặt lại mật khẩu**.</span><span class="sxs-lookup"><span data-stu-id="11939-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="11939-147">Làm theo hướng dẫn trên màn hình.</span><span class="sxs-lookup"><span data-stu-id="11939-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="11939-148">Chỉ Reset được thực hiện thông qua dịch vụ hỗ trợ Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="11939-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="11939-149">**Tôi đặt lại mật khẩu người dùng tại cơ sở từ cổng thông tin quản trị Office 365 hoặc ứng dụng Office 365 dành cho thiết bị di động nhưng người dùng vẫn không thể đăng nhập**</span><span class="sxs-lookup"><span data-stu-id="11939-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="11939-150">Không hỗ trợ mật khẩu của Writeback trong cổng thông tin này.</span><span class="sxs-lookup"><span data-stu-id="11939-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="11939-151">Đặt lại mật khẩu người dùng một lần nữa trong cổng thông tin Azure-portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="11939-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

