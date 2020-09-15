---
title: Thay đổi quyền thư mục công cộng
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: a2a902e8fdfd8628772364c173979c633d25a169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714269"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="f2236-102">Thay đổi quyền thư mục công cộng</span><span class="sxs-lookup"><span data-stu-id="f2236-102">Changing public folder permissions</span></span>

<span data-ttu-id="f2236-103">Quyền đối với thư mục công cộng có thể thay đổi bởi người dùng và người quản trị trong Outlook.</span><span class="sxs-lookup"><span data-stu-id="f2236-103">Public folder permissions can be changed by users and administrators in Outlook.</span></span> <span data-ttu-id="f2236-104">Người quản trị cũng có thể kiểm soát quyền từ Trung tâm quản trị Exchange (EAC), bằng cách thực hiện như sau:</span><span class="sxs-lookup"><span data-stu-id="f2236-104">Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="f2236-105">Trong Trung tâm quản trị Microsoft 365, hãy đi đến Exchange **Trung tâm quản trị** \> **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="f2236-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="f2236-106">Chọn các **thư mục công cộng**.</span><span class="sxs-lookup"><span data-stu-id="f2236-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="f2236-107">Từ đó, bạn có thể thay đổi quyền cho các thư mục công cộng riêng lẻ bằng cách gán các nhóm bảo mật thành các quyền.</span><span class="sxs-lookup"><span data-stu-id="f2236-107">From there, you can change permissions for individual public folders by assigning security groups to permissions.</span></span> <span data-ttu-id="f2236-108">Đối với người dùng cuối để thay đổi quyền thư mục công cộng, người dùng cần có quyền chủ sở hữu trên thư mục.</span><span class="sxs-lookup"><span data-stu-id="f2236-108">For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

<span data-ttu-id="f2236-109">Vui lòng làm theo quy trình được mô tả trong [cách chẩn đoán và khắc phục các vấn đề cấp phép thư mục công cộng](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) để khắc phục sự cố quyền đối với thư mục công cộng.</span><span class="sxs-lookup"><span data-stu-id="f2236-109">Please follow the procedure described in [How to diagnose and fix public folder permission issues](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) to troubleshoot public folder permission issues.</span></span>

<span data-ttu-id="f2236-110">**Lưu ý**: có một số vấn đề đã biết mà bạn có thể gặp phải khi bạn tìm cách thay đổi quyền trên thư mục công cộng.</span><span class="sxs-lookup"><span data-stu-id="f2236-110">**Note**: There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="f2236-111">Xem các bài viết sau để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="f2236-111">See the following articles for more information.</span></span>

- [<span data-ttu-id="f2236-112">Không thể áp dụng quyền đối với các thư mục thư mục công cộng trong EAC</span><span class="sxs-lookup"><span data-stu-id="f2236-112">Can't apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- [<span data-ttu-id="f2236-113">Lỗi "không tìm thấy hộp thư trong vùng rừng cục bộ" khi bạn truy nhập vào các thư mục công cộng</span><span class="sxs-lookup"><span data-stu-id="f2236-113">"The mailbox is not found in the local forest" error when you access public folders</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
