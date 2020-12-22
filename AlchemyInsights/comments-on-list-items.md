---
title: Chú thích về các mục trong danh sách
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724176"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="58824-102">Chú thích về các mục trong danh sách</span><span class="sxs-lookup"><span data-stu-id="58824-102">Comments on List items</span></span>

<span data-ttu-id="58824-103">Người dùng có thể xem tất cả chú thích trên mục danh sách và bộ lọc giữa các dạng xem Hiển thị chú thích hoặc hoạt động liên quan đến một mục.</span><span class="sxs-lookup"><span data-stu-id="58824-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="58824-104">Người dùng cần lưu ý những điều sau đây trước khi có thể thêm và xóa chú thích:</span><span class="sxs-lookup"><span data-stu-id="58824-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="58824-105">Chú thích theo các thiết đặt quyền vốn có trong SharePoint.</span><span class="sxs-lookup"><span data-stu-id="58824-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="58824-106">Các danh sách cổ điển chưa được xây dựng để hiển thị trong giao diện người dùng hiện đại, chẳng hạn như danh sách nhiệm vụ, sẽ không có tính năng chú thích này.</span><span class="sxs-lookup"><span data-stu-id="58824-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="58824-107">Chú thích trong các danh sách trong nhóm không sẵn dùng với bản phát hành này.</span><span class="sxs-lookup"><span data-stu-id="58824-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="58824-108">Chú thích không được lập chỉ mục theo tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="58824-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="58824-109">Người quản trị có thể tắt tính năng này ở cấp độ tổ chức bằng cách thay đổi tham số **Commentsonlistitemsdisabled** trong lệnh ghép ngắn **Set-spothuê** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="58824-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="58824-110">Hiện tại bạn không thể tắt cho chú thích ở mức trang hoặc danh sách.</span><span class="sxs-lookup"><span data-stu-id="58824-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="58824-111">Chúng tôi hy vọng sẽ có những điều khiển này trong bản Cập Nhật sau này, có khả năng là quý i đầu tiên 2021.</span><span class="sxs-lookup"><span data-stu-id="58824-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
