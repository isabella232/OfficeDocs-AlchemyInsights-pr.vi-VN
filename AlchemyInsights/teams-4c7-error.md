---
title: Lỗi teams 4c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796472"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="2f785-102">lỗi 4c7 trong Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="2f785-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="2f785-103">Lỗi này xảy ra do Microsoft teams yêu cầu xác thực biểu mẫu.</span><span class="sxs-lookup"><span data-stu-id="2f785-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="2f785-104">Khi bạn triển khai dịch vụ liên kết Active Directory (AD FS), hình thức xác thực không được kích hoạt cho mạng nội bộ theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="2f785-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="2f785-105">Nếu xác thực tích hợp Windows không thành công, bạn được nhắc đăng nhập bằng cách sử dụng xác thực biểu mẫu.</span><span class="sxs-lookup"><span data-stu-id="2f785-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="2f785-106">Để giải quyết vấn đề này, cho phép hình thức xác thực bằng cách sử dụng AD FS Microsoft Management Console (MMC) đính vào trên máy tính có bản sao cục bộ của Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2f785-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="2f785-107">Caranya sebagai berikut:</span><span class="sxs-lookup"><span data-stu-id="2f785-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="2f785-108">Trong ngăn điều hướng, duyệt đến **chính sách xác thực**.</span><span class="sxs-lookup"><span data-stu-id="2f785-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="2f785-109">Trong **hành động** trong ngăn chi tiết, chọn **chỉnh sửa xác thực chính toàn cầu**.</span><span class="sxs-lookup"><span data-stu-id="2f785-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="2f785-110">Trên tab **intranet** , chọn **hình thức xác thực**.</span><span class="sxs-lookup"><span data-stu-id="2f785-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="2f785-111">Chọn **OK** (hoặc **áp dụng**).</span><span class="sxs-lookup"><span data-stu-id="2f785-111">Select **OK** (or **Apply**).</span></span>