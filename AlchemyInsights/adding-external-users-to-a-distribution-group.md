---
title: Thêm người dùng bên ngoài cho một nhóm phân phối
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 641636add2069fc395df9af156d8c011493a634a
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/29/2019
ms.locfileid: "36660814"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="3fcfc-102">Thêm người dùng bên ngoài cho một nhóm phân phối</span><span class="sxs-lookup"><span data-stu-id="3fcfc-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="3fcfc-103">Thêm một số liên lạc bên ngoài cho một nhóm phân phối (DG) là một quá trình hai bước:</span><span class="sxs-lookup"><span data-stu-id="3fcfc-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="3fcfc-104">Tạo số liên lạc thư cho người dùng bên ngoài:</span><span class="sxs-lookup"><span data-stu-id="3fcfc-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="3fcfc-105">Trong Trung tâm quản trị, đi tới **người dùng** > [địa chỉ liên lạc](https://admin.microsoft.com/adminportal/home#/Contact) trang.</span><span class="sxs-lookup"><span data-stu-id="3fcfc-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="3fcfc-106">Chọn **Thêm số liên lạc**.</span><span class="sxs-lookup"><span data-stu-id="3fcfc-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="3fcfc-107">Nhập các thông tin liên hệ của bạn và chọn **Thêm**.</span><span class="sxs-lookup"><span data-stu-id="3fcfc-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="3fcfc-108">Địa chỉ liên lạc qua thư để DG của bạn:</span><span class="sxs-lookup"><span data-stu-id="3fcfc-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="3fcfc-109">Trong Trung tâm quản trị, đi đến các **nhóm** > [nhóm](https://admin.microsoft.com/adminportal/home#/groups) trang.</span><span class="sxs-lookup"><span data-stu-id="3fcfc-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="3fcfc-110">Tìm DG bạn muốn thêm người dùng bên ngoài, và chọn để mở hộp thoại chỉnh sửa.</span><span class="sxs-lookup"><span data-stu-id="3fcfc-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="3fcfc-111">Trên tab **thành viên** , hãy chọn **xem tất cả và quản lý các thành viên**.</span><span class="sxs-lookup"><span data-stu-id="3fcfc-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="3fcfc-112">Chọn **thêm thành viên**.</span><span class="sxs-lookup"><span data-stu-id="3fcfc-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="3fcfc-113">Chọn số liên lạc thư bạn đã tạo trên bước trước, và sau đó chọn **Save**.</span><span class="sxs-lookup"><span data-stu-id="3fcfc-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="3fcfc-114">Nếu sau khi làm theo các bước sau người dùng bên ngoài của bạn không thể gửi email cho DG hoặc không nhận được email từ nó, nó có thể là DG được đánh dấu để chỉ cho phép các email từ người dùng nội bộ.</span><span class="sxs-lookup"><span data-stu-id="3fcfc-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="3fcfc-115">Bạn có thể kiểm tra cấu hình này và sửa chữa nó theo các chỉ dẫn [dưới đây](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span><span class="sxs-lookup"><span data-stu-id="3fcfc-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="3fcfc-116">**Lưu ý:** Những hướng dẫn này không áp dụng nếu loại của nhóm là "Nhóm Office 365" thay vì "Nhóm phân phối."</span><span class="sxs-lookup"><span data-stu-id="3fcfc-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="3fcfc-117">Nếu trường hợp đó xảy ra, bạn có thể thêm người dùng bên ngoài trực tiếp vào nhóm từ Outlook.</span><span class="sxs-lookup"><span data-stu-id="3fcfc-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="3fcfc-118">Các thông tin chi tiết về Office 365 nhóm khách cũng như các hướng dẫn để Thêm khách bên ngoài có thể được tìm thấy trong [bài viết này](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="3fcfc-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  