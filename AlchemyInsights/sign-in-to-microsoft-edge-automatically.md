---
title: Tự động đăng nhập vào Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678821"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="ac9a4-102">Tự động đăng nhập vào Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="ac9a4-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="ac9a4-103">Microsoft Edge sử dụng tài khoản mặc định của OS để tự động đăng nhập vào người dùng theo cách cấu hình thiết bị của người dùng.</span><span class="sxs-lookup"><span data-stu-id="ac9a4-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="ac9a4-104">Các kịch bản của từng kiểu cấu hình thiết bị và quy trình đăng nhập người dùng phụ thuộc của nó được mô tả dưới đây:</span><span class="sxs-lookup"><span data-stu-id="ac9a4-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="ac9a4-105">**Thiết bị được kết hợp/đọc-J**: tùy chọn này có sẵn trên Windows 10, xuống mức Windows và các phiên bản máy chủ tương ứng.</span><span class="sxs-lookup"><span data-stu-id="ac9a4-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="ac9a4-106">Người dùng được tự động đăng nhập bằng tài khoản Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="ac9a4-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="ac9a4-107">**Thiết bị được nối tên miền**: tùy chọn này sẵn có trên Windows 10, xuống mức Windows và các phiên bản máy chủ tương ứng.</span><span class="sxs-lookup"><span data-stu-id="ac9a4-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="ac9a4-108">Theo mặc định, người dùng có tài khoản miền không được tự động đăng nhập; để kích hoạt tính năng đăng nhập tự động cho họ, hãy sử dụng chính sách **ConfigureOnPremisesAccountAutoSignIn** .</span><span class="sxs-lookup"><span data-stu-id="ac9a4-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="ac9a4-109">Để kích hoạt tính năng đăng nhập tự động cho người dùng bằng tài khoản Azure AD, hãy cân nhắc việc gia nhập kết hợp thiết bị của họ.</span><span class="sxs-lookup"><span data-stu-id="ac9a4-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="ac9a4-110">**Tài khoản mặc định của hệ điều hành là tài khoản Microsoft**: tùy chọn này sẵn dùng trên Windows 10 RS3 (phiên bản 1709, bản dựng 10.0.16299) và các phiên bản mới hơn.</span><span class="sxs-lookup"><span data-stu-id="ac9a4-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="ac9a4-111">Kịch bản dường như không xảy ra trên các thiết bị doanh nghiệp.</span><span class="sxs-lookup"><span data-stu-id="ac9a4-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="ac9a4-112">Tuy nhiên, nếu tài khoản mặc định của hệ điều hành là tài khoản Microsoft, thì Microsoft Edge sẽ tự động đăng nhập vào người dùng bằng tài khoản Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ac9a4-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
