---
title: Teams bổ trợ dành cho máy Mac
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
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582092"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="6830d-102">Teams bổ trợ dành cho máy Mac</span><span class="sxs-lookup"><span data-stu-id="6830d-102">Teams add-in for Mac</span></span>

<span data-ttu-id="6830d-103">Để khắc phục sự cố bổ trợ Teams dành cho người dùng hệ điều hành Mac bị thiếu, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="6830d-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="6830d-104">**Bước 1:** Nếu bạn có tùy chọn Kết hợp Exchange tại chỗ (2016 CU3 trở lên), hãy sử dụng công cụ Test-HMA.ps1 để xác nhận rằng Xác thực Hiện đại Kết hợp được đặt cấu hình đúng cách.</span><span class="sxs-lookup"><span data-stu-id="6830d-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="6830d-105">Để biết thêm thông tin, xem mục Xác thực Xác thực Hiện đại Kết hợp [cho Outlook cho iOS và Android.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="6830d-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="6830d-106">**Lưu ý** Sử dụng định dạng địa chỉ UPN (ví dụ: [username@contoso.com](mailto:username@contoso.com)), không phải tên miền\tên người dùng.</span><span class="sxs-lookup"><span data-stu-id="6830d-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="6830d-107">Thực hiện việc này ngay cả đối với người Exchange Online thư của họ.</span><span class="sxs-lookup"><span data-stu-id="6830d-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="6830d-108">**Bước 2:** Để người dùng đi tới Tài **khoản**  >  **Công cụ**... trong Outlook for Mac và tìm và chọn tài khoản.</span><span class="sxs-lookup"><span data-stu-id="6830d-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="6830d-109">Xác nhận tên người dùng được liệt kê có định dạng UPN (ví [dụ: username@contoso.com).](mailto:username@contoso.com)</span><span class="sxs-lookup"><span data-stu-id="6830d-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="6830d-110">**Bước 3:** Xác nhận người dùng đã được cấp phép Microsoft Teams dùng.</span><span class="sxs-lookup"><span data-stu-id="6830d-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="6830d-111">Người dùng phải đang sử dụng đăng ký Office 365 cho máy Mac, phiên bản sản phẩm 16.24 trở lên.</span><span class="sxs-lookup"><span data-stu-id="6830d-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>