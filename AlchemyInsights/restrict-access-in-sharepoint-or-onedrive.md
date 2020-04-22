---
title: Hạn chế quyền truy cập trong SharePoint hoặc OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715906"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="f28d7-102">Hạn chế quyền truy cập trong SharePoint hoặc OneDrive</span><span class="sxs-lookup"><span data-stu-id="f28d7-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="f28d7-103">Trong SharePoint và OneDrive, bạn hạn chế quyền truy cập vào các mục như tệp, thư mục và danh sách bằng cách cấp quyền truy cập chỉ cho các nhóm hoặc cá nhân bạn muốn có quyền truy cập.</span><span class="sxs-lookup"><span data-stu-id="f28d7-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="f28d7-104">Theo mặc định, quyền trong SharePoint được kế thừa từ cao hơn trong hệ thống phân cấp.</span><span class="sxs-lookup"><span data-stu-id="f28d7-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="f28d7-105">Vì vậy, một tệp kế thừa các quyền của nó từ thư mục, kế thừa các quyền của nó từ thư viện, kế thừa các quyền từ trang web.</span><span class="sxs-lookup"><span data-stu-id="f28d7-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="f28d7-106">Bạn có thể chia sẻ ở một mức độ cao hơn (chẳng hạn như bằng cách chia sẻ toàn bộ trang web) và sau đó phá vỡ thừa kế nếu bạn không muốn chia sẻ tất cả các mục trên trang web.</span><span class="sxs-lookup"><span data-stu-id="f28d7-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="f28d7-107">Tuy nhiên, chúng tôi không khuyên bạn nên điều này vì nó làm cho việc duy trì các quyền phức tạp hơn và khó hiểu trong tương lai.</span><span class="sxs-lookup"><span data-stu-id="f28d7-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="f28d7-108">Đây là những gì bạn có thể làm thay vì:</span><span class="sxs-lookup"><span data-stu-id="f28d7-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="f28d7-109">Ví dụ: nếu bạn muốn chia sẻ tất cả nội dung của thư mục ngoại trừ một tệp trong đó, hãy di chuyển tệp đó sang vị trí mới không được chia sẻ.</span><span class="sxs-lookup"><span data-stu-id="f28d7-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="f28d7-110">Nếu bạn có hai cặp con trong một thư mục, và bạn muốn chia sẻ một cặp với nhóm A và B và cho phép chỉ nhóm quyền truy cập vào thư mục con thứ hai, hãy chia sẻ cặp cha với nhóm A và thêm nhóm B vào con đầu tiên.</span><span class="sxs-lookup"><span data-stu-id="f28d7-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="f28d7-111">Dừng chia sẻ tệp hoặc thư mục</span><span class="sxs-lookup"><span data-stu-id="f28d7-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

