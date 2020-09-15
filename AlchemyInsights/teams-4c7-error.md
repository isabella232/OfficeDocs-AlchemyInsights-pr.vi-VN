---
title: Lỗi nhóm 6c 7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700225"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="0006b-102">lỗi 6x7 trong Microsoft nhóm</span><span class="sxs-lookup"><span data-stu-id="0006b-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="0006b-103">Lỗi này xảy ra vì Microsoft nhóm yêu cầu xác thực biểu mẫu.</span><span class="sxs-lookup"><span data-stu-id="0006b-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="0006b-104">Khi bạn triển khai các dịch vụ liên kết Active Directory (AD FS), xác thực biểu mẫu không được kích hoạt cho mạng nội bộ theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="0006b-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="0006b-105">Nếu xác thực tích hợp Windows không thành công, bạn sẽ được nhắc đăng nhập bằng cách sử dụng xác thực biểu mẫu.</span><span class="sxs-lookup"><span data-stu-id="0006b-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="0006b-106">Để giải quyết sự cố này, hãy bật xác thực biểu mẫu bằng cách sử dụng trình điều khiển Microsoft Management Console (MMC) của AD FS trên máy tính có bản sao cục bộ của Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0006b-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="0006b-107">Caranya sebagai berikut:</span><span class="sxs-lookup"><span data-stu-id="0006b-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="0006b-108">Trong ngăn dẫn hướng, duyệt đến **chính sách xác thực**.</span><span class="sxs-lookup"><span data-stu-id="0006b-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="0006b-109">Bên dưới **hành động** trong ngăn chi tiết, hãy chọn **chỉnh sửa xác thực toàn cầu chính**.</span><span class="sxs-lookup"><span data-stu-id="0006b-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="0006b-110">Trên tab **intranet** , chọn **biểu mẫu xác thực**.</span><span class="sxs-lookup"><span data-stu-id="0006b-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="0006b-111">Chọn **OK** (hoặc **áp dụng**).</span><span class="sxs-lookup"><span data-stu-id="0006b-111">Select **OK** (or **Apply**).</span></span>