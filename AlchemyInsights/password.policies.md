---
title: Chính sách mật khẩu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747058"
---
# <a name="password-policies"></a><span data-ttu-id="2b240-102">Chính sách mật khẩu</span><span class="sxs-lookup"><span data-stu-id="2b240-102">Password policies</span></span>

<span data-ttu-id="2b240-103">**Tôi đang gặp vấn đề với chính sách mật khẩu cho người dùng**</span><span class="sxs-lookup"><span data-stu-id="2b240-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="2b240-104">Chính sách mật khẩu cho người dùng tùy thuộc vào việc người dùng chỉ có trên điện toán đám mây hoặc tại chỗ.</span><span class="sxs-lookup"><span data-stu-id="2b240-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="2b240-105">Chỉ đám mây người dùng phải chọn một mật khẩu đáp ứng các yêu cầu trong bài viết này: [chính sách mật khẩu chỉ áp dụng cho tài khoản người dùng đám mây](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="2b240-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="2b240-106">Người dùng tại cơ sở phải chọn một mật khẩu đáp ứng các yêu cầu tại chỗ.</span><span class="sxs-lookup"><span data-stu-id="2b240-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="2b240-107">Nếu người dùng tại cơ sở không thể đặt mật khẩu của mình, hãy kiểm tra các yêu cầu tại chỗ của bạn.</span><span class="sxs-lookup"><span data-stu-id="2b240-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="2b240-108">**Tôi không biết cách đặt hoặc kiểm tra chính sách hết hạn mật khẩu**</span><span class="sxs-lookup"><span data-stu-id="2b240-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="2b240-109">Bạn có thể đặt và kiểm tra chính sách hết hạn cho người dùng đám mây trong đối tượng thuê của mình bằng cách sử dụng PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2b240-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="2b240-110">Làm theo các hướng dẫn trong bài viết này: [đặt hoặc kiểm tra chính sách mật khẩu bằng cách sử dụng PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="2b240-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="2b240-111">Chính sách hết hạn mật khẩu cho người dùng tại cơ sở được đặt trong quảng cáo tại cơ sở của bạn.</span><span class="sxs-lookup"><span data-stu-id="2b240-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="2b240-112">**Các nối kết hữu ích khác:**</span><span class="sxs-lookup"><span data-stu-id="2b240-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="2b240-113">Bắt đầu với việc đặt lại mật khẩu</span><span class="sxs-lookup"><span data-stu-id="2b240-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="2b240-114">Khắc phục sự cố đặt lại mật khẩu khởi tạo người quản trị</span><span class="sxs-lookup"><span data-stu-id="2b240-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
