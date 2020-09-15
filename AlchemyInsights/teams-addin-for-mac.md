---
title: Bổ trợ nhóm cho Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670350"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="11bb0-102">Bổ trợ nhóm cho Mac</span><span class="sxs-lookup"><span data-stu-id="11bb0-102">Teams add-in for Mac</span></span>

<span data-ttu-id="11bb0-103">Để khắc phục sự cố dành cho các bổ trợ nhóm không bị thiếu cho người dùng hệ điều hành Mac, hãy làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="11bb0-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="11bb0-104">**Bước 1:** Nếu bạn có kết hợp Exchange tại cơ sở (2016 CU3 hoặc phiên bản mới hơn), hãy sử dụng công cụ Test-HMA.ps1 để xác nhận rằng kết hợp xác thực hiện đại sẽ được cấu hình đúng.</span><span class="sxs-lookup"><span data-stu-id="11bb0-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="11bb0-105">Để biết thêm thông tin, hãy xem mục [phê chuẩn thiết lập xác thực hiện đại cho Outlook for iOS và Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="11bb0-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="11bb0-106">**Ghi chú** Sử dụng định dạng địa chỉ UPN (ví dụ, [username@contoso.com](mailto:username@contoso.com)), không phải là \ tên người dùng.</span><span class="sxs-lookup"><span data-stu-id="11bb0-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="11bb0-107">Hãy làm điều này ngay cả đối với người dùng với hộp thư Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="11bb0-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="11bb0-108">**Bước 2:** Người dùng đã đi đến **Tools**các  >  **tài khoản**công cụ... trong Outlook for Mac, và tìm và chọn tài khoản.</span><span class="sxs-lookup"><span data-stu-id="11bb0-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="11bb0-109">Xác nhận tên người dùng được liệt kê ở định dạng UPN (ví dụ, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="11bb0-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="11bb0-110">**Bước 3:** Xác nhận người dùng là người dùng Microsoft nhóm được cấp phép.</span><span class="sxs-lookup"><span data-stu-id="11bb0-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="11bb0-111">Người dùng phải sử dụng đăng ký Office 365 cho máy Mac, phiên bản sản phẩm 16,24 hoặc mới hơn.</span><span class="sxs-lookup"><span data-stu-id="11bb0-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>