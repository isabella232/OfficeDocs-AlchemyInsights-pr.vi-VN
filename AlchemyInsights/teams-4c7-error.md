---
title: Lỗi nhóm 6c 7
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786691"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="1ebc2-102">lỗi 6x7 trong Microsoft nhóm</span><span class="sxs-lookup"><span data-stu-id="1ebc2-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="1ebc2-103">Lỗi này xảy ra vì Microsoft nhóm yêu cầu xác thực biểu mẫu.</span><span class="sxs-lookup"><span data-stu-id="1ebc2-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="1ebc2-104">Khi bạn triển khai các dịch vụ liên kết Active Directory (AD FS), xác thực biểu mẫu không được kích hoạt cho mạng nội bộ theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="1ebc2-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="1ebc2-105">Nếu xác thực tích hợp Windows không thành công, bạn sẽ được nhắc đăng nhập bằng cách sử dụng xác thực biểu mẫu.</span><span class="sxs-lookup"><span data-stu-id="1ebc2-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="1ebc2-106">Để giải quyết sự cố này, hãy bật xác thực biểu mẫu bằng cách sử dụng trình điều khiển Microsoft Management Console (MMC) của AD FS trên máy tính có bản sao cục bộ của Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1ebc2-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="1ebc2-107">Caranya sebagai berikut:</span><span class="sxs-lookup"><span data-stu-id="1ebc2-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="1ebc2-108">Trong ngăn dẫn hướng, duyệt đến **chính sách xác thực**.</span><span class="sxs-lookup"><span data-stu-id="1ebc2-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="1ebc2-109">Bên dưới **hành động** trong ngăn chi tiết, hãy chọn **chỉnh sửa xác thực toàn cầu chính**.</span><span class="sxs-lookup"><span data-stu-id="1ebc2-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="1ebc2-110">Trên tab **intranet** , chọn **biểu mẫu xác thực**.</span><span class="sxs-lookup"><span data-stu-id="1ebc2-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="1ebc2-111">Chọn **OK** (hoặc **áp dụng**).</span><span class="sxs-lookup"><span data-stu-id="1ebc2-111">Select **OK** (or **Apply**).</span></span>