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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982552"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="1e08d-102">Chú thích về các mục trong danh sách</span><span class="sxs-lookup"><span data-stu-id="1e08d-102">Comments on List items</span></span>

<span data-ttu-id="1e08d-103">Người dùng sẽ sớm có thể thêm và xóa bỏ chú thích trong danh sách mục.</span><span class="sxs-lookup"><span data-stu-id="1e08d-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="1e08d-104">Người dùng có thể xem tất cả chú thích trên mục danh sách và bộ lọc giữa các dạng xem Hiển thị chú thích hoặc hoạt động liên quan đến một mục.</span><span class="sxs-lookup"><span data-stu-id="1e08d-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="1e08d-105">**Thời gian** :</span><span class="sxs-lookup"><span data-stu-id="1e08d-105">**Timing** :</span></span>

<span data-ttu-id="1e08d-106">**Bản phát hành mục tiêu** : dần dần triển khai vào giữa tháng mười và dự kiến sẽ hoàn thành vào giữa tháng mười một</span><span class="sxs-lookup"><span data-stu-id="1e08d-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="1e08d-107">**Bản phát hành tiêu chuẩn** : đã từng bước đầu tiên vào giữa tháng mười một và dự kiến sẽ hoàn thành vào tháng mười hai</span><span class="sxs-lookup"><span data-stu-id="1e08d-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="1e08d-108">Triển **khai: bản** phát hành mục tiêu cho toàn bộ tổ chức</span><span class="sxs-lookup"><span data-stu-id="1e08d-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="1e08d-109">Người dùng cần lưu ý những điều sau đây trước khi có thể thêm và xóa chú thích:</span><span class="sxs-lookup"><span data-stu-id="1e08d-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="1e08d-110">Chú thích theo các thiết đặt quyền vốn có trong SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1e08d-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="1e08d-111">Các danh sách cổ điển chưa được xây dựng để hiển thị trong giao diện người dùng hiện đại, chẳng hạn như danh sách nhiệm vụ, sẽ không có tính năng chú thích này.</span><span class="sxs-lookup"><span data-stu-id="1e08d-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="1e08d-112">Chú thích trong các danh sách trong nhóm không sẵn dùng với bản phát hành này.</span><span class="sxs-lookup"><span data-stu-id="1e08d-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="1e08d-113">Chú thích không được lập chỉ mục theo tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="1e08d-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="1e08d-114">Người quản trị có thể tắt tính năng này ở cấp độ tổ chức bằng cách thay đổi tham số **Commentsonlistitemsdisabled** trong lệnh ghép ngắn **Set-spothuê** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1e08d-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="1e08d-115">Hiện tại bạn không thể tắt cho chú thích ở mức trang hoặc danh sách.</span><span class="sxs-lookup"><span data-stu-id="1e08d-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="1e08d-116">Chúng tôi hy vọng sẽ có những điều khiển này trong bản Cập Nhật sau này, có khả năng là quý i đầu tiên 2021.</span><span class="sxs-lookup"><span data-stu-id="1e08d-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
