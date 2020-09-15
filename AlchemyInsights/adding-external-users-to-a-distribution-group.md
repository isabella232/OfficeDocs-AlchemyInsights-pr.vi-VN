---
title: Thêm người dùng bên ngoài vào một nhóm phân phối
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663535"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="dcdf7-102">Thêm người dùng bên ngoài vào một nhóm phân phối</span><span class="sxs-lookup"><span data-stu-id="dcdf7-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="dcdf7-103">Thêm một liên hệ bên ngoài vào một nhóm phân phối (DG) là quy trình hai bước:</span><span class="sxs-lookup"><span data-stu-id="dcdf7-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="dcdf7-104">Tạo liên hệ thư cho người dùng bên ngoài:</span><span class="sxs-lookup"><span data-stu-id="dcdf7-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="dcdf7-105">Trong Trung tâm quản trị, đi tới **Users**  >  trang[liên hệ](https://admin.microsoft.com/adminportal/home#/Contact) của người dùng.</span><span class="sxs-lookup"><span data-stu-id="dcdf7-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="dcdf7-106">Chọn **Thêm liên hệ**.</span><span class="sxs-lookup"><span data-stu-id="dcdf7-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="dcdf7-107">Nhập thông tin cho liên hệ của bạn, rồi chọn **Thêm**.</span><span class="sxs-lookup"><span data-stu-id="dcdf7-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="dcdf7-108">Thêm liên hệ thư vào DG của bạn:</span><span class="sxs-lookup"><span data-stu-id="dcdf7-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="dcdf7-109">Trong Trung tâm quản trị, đi tới **Groups**  >  trang[nhóm](https://admin.microsoft.com/adminportal/home#/groups) nhóm.</span><span class="sxs-lookup"><span data-stu-id="dcdf7-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="dcdf7-110">Tìm DG bạn muốn thêm người dùng bên ngoài, rồi chọn nó để mở hộp thoại chỉnh sửa.</span><span class="sxs-lookup"><span data-stu-id="dcdf7-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="dcdf7-111">Trên tab **thành viên** , hãy chọn **xem tất cả và quản lý thành viên**.</span><span class="sxs-lookup"><span data-stu-id="dcdf7-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="dcdf7-112">Chọn **thêm thành viên**.</span><span class="sxs-lookup"><span data-stu-id="dcdf7-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="dcdf7-113">Chọn liên hệ thư bạn đã tạo ở bước trước, rồi chọn **lưu**.</span><span class="sxs-lookup"><span data-stu-id="dcdf7-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="dcdf7-114">Nếu sau khi làm theo các bước này, người dùng bên ngoài của bạn không thể gửi email đến DG hoặc không nhận được email từ nó, thì có thể là DG được đánh dấu là chỉ cho phép các email từ người dùng nội bộ.</span><span class="sxs-lookup"><span data-stu-id="dcdf7-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="dcdf7-115">Bạn có thể kiểm tra cấu hình này và sửa nó theo các hướng dẫn [ở đây](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="dcdf7-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="dcdf7-116">**Lưu ý:** Những hướng dẫn này không áp dụng nếu loại nhóm của bạn là "nhóm Microsoft 365" thay vì "nhóm phân phối".</span><span class="sxs-lookup"><span data-stu-id="dcdf7-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="dcdf7-117">Nếu đó là trường hợp, bạn có thể thêm người dùng bên ngoài trực tiếp vào nhóm từ Outlook.</span><span class="sxs-lookup"><span data-stu-id="dcdf7-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="dcdf7-118">Thông tin chi tiết về các nhóm Microsoft 365 cũng như các hướng dẫn cho việc thêm khách bên ngoài có thể tìm thấy trong [bài viết này](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="dcdf7-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  