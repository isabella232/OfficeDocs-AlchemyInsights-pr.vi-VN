---
title: Chặn các chữ ký email đã tạo bằng người dùng
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243763"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="fef12-102">Chặn các chữ ký email đã tạo bằng người dùng</span><span class="sxs-lookup"><span data-stu-id="fef12-102">Block user-made email signatures</span></span>

<span data-ttu-id="fef12-103">Giải pháp sau đây chỉ áp dụng cho chữ ký email được tạo trong Outlook trên web.</span><span class="sxs-lookup"><span data-stu-id="fef12-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="fef12-104">Bạn chỉ có thể chặn các chữ ký trong ứng dụng Outlook nếu bạn có máy chủ Exchange tại cơ sở.</span><span class="sxs-lookup"><span data-stu-id="fef12-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="fef12-105">Trong Trung tâm quản trị, chọn Exchange **Trung tâm quản trị**  >  .</span><span class="sxs-lookup"><span data-stu-id="fef12-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="fef12-106">Bấm vào **quyền** của  >  **chính sách Outlook Web App**.</span><span class="sxs-lookup"><span data-stu-id="fef12-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="fef12-107">Chọn chính sách, rồi bấm vào biểu tượng bút chì để sửa nó.</span><span class="sxs-lookup"><span data-stu-id="fef12-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="fef12-108">Bấm vào **tính năng**  >  **Thêm tùy chọn**.</span><span class="sxs-lookup"><span data-stu-id="fef12-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="fef12-109">Bên dưới **trải nghiệm người dùng**, xóa hộp kiểm **chữ ký email** , rồi bấm **lưu**.</span><span class="sxs-lookup"><span data-stu-id="fef12-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="fef12-110">**Quan trọng:** Nếu đã thêm chữ ký trước khi xóa hộp kiểm này, người dùng sẽ vẫn có thể sử dụng.</span><span class="sxs-lookup"><span data-stu-id="fef12-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="fef12-111">Yêu cầu họ loại bỏ nó.</span><span class="sxs-lookup"><span data-stu-id="fef12-111">Ask them to remove it.</span></span>
