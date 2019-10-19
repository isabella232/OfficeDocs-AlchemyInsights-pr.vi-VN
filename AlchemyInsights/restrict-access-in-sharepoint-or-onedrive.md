---
title: Hạn chế quyền truy cập trong SharePoint hoặc OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551473"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="1eca4-102">Hạn chế quyền truy cập trong SharePoint hoặc OneDrive</span><span class="sxs-lookup"><span data-stu-id="1eca4-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="1eca4-103">Trong SharePoint và OneDrive, bạn hạn chế quyền truy cập vào các mục như tệp, thư mục và danh sách bằng cách cấp quyền truy cập chỉ cho các nhóm hoặc cá nhân bạn muốn có quyền truy cập.</span><span class="sxs-lookup"><span data-stu-id="1eca4-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="1eca4-104">Theo mặc định, quyền trong SharePoint được kế thừa từ cao hơn trong hệ thống phân cấp.</span><span class="sxs-lookup"><span data-stu-id="1eca4-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="1eca4-105">Vì vậy, một tệp kế thừa các quyền của nó từ thư mục, kế thừa các quyền của nó từ thư viện, kế thừa các quyền từ trang web.</span><span class="sxs-lookup"><span data-stu-id="1eca4-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="1eca4-106">Bạn có thể chia sẻ ở một mức độ cao hơn (chẳng hạn như bằng cách chia sẻ toàn bộ trang web) và sau đó phá vỡ thừa kế nếu bạn không muốn chia sẻ tất cả các mục trên trang web.</span><span class="sxs-lookup"><span data-stu-id="1eca4-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="1eca4-107">Tuy nhiên, chúng tôi không khuyên bạn nên điều này vì nó làm cho việc duy trì các quyền phức tạp hơn và khó hiểu trong tương lai.</span><span class="sxs-lookup"><span data-stu-id="1eca4-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="1eca4-108">Đây là những gì bạn có thể làm thay vì:</span><span class="sxs-lookup"><span data-stu-id="1eca4-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="1eca4-109">Ví dụ: nếu bạn muốn chia sẻ tất cả nội dung của thư mục ngoại trừ một tệp trong đó, hãy di chuyển tệp đó sang vị trí mới không được chia sẻ.</span><span class="sxs-lookup"><span data-stu-id="1eca4-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="1eca4-110">Nếu bạn có hai cặp con trong một thư mục, và bạn muốn chia sẻ một cặp với nhóm A và B và cho phép chỉ nhóm quyền truy cập vào thư mục con thứ hai, hãy chia sẻ cặp cha với nhóm A và thêm nhóm B vào con đầu tiên.</span><span class="sxs-lookup"><span data-stu-id="1eca4-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="1eca4-111">Dừng chia sẻ tệp hoặc thư mục</span><span class="sxs-lookup"><span data-stu-id="1eca4-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

