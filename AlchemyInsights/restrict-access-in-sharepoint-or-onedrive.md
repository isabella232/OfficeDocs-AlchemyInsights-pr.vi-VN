---
title: Hạn chế quyền truy nhập trong SharePoint hoặc OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720704"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="725fa-102">Hạn chế quyền truy nhập trong SharePoint hoặc OneDrive</span><span class="sxs-lookup"><span data-stu-id="725fa-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="725fa-103">Trong SharePoint và OneDrive, bạn hạn chế quyền truy nhập vào các mục như tệp, thư mục và danh sách bằng cách cấp quyền truy nhập chỉ cho các nhóm hoặc cá nhân mà bạn muốn có quyền truy nhập.</span><span class="sxs-lookup"><span data-stu-id="725fa-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="725fa-104">Theo mặc định, các quyền trong SharePoint được kế thừa từ cao hơn trong cấu trúc phân cấp.</span><span class="sxs-lookup"><span data-stu-id="725fa-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="725fa-105">Vì vậy, một tệp đã thừa kế quyền của nó từ thư mục, vốn thừa kế quyền của nó từ thư viện, vốn sẽ thừa kế quyền của nó từ site đó.</span><span class="sxs-lookup"><span data-stu-id="725fa-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="725fa-106">Bạn có thể chia sẻ ở mức cao hơn (chẳng hạn như bằng cách chia sẻ toàn bộ trang) và sau đó ngắt kế thừa nếu bạn không muốn chia sẻ tất cả các mục trên trang web.</span><span class="sxs-lookup"><span data-stu-id="725fa-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="725fa-107">Tuy nhiên, chúng tôi không khuyên bạn nên điều này vì việc duy trì quyền phức tạp hơn và khó hiểu hơn trong tương lai.</span><span class="sxs-lookup"><span data-stu-id="725fa-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="725fa-108">Sau đây là những gì bạn có thể thực hiện thay thế:</span><span class="sxs-lookup"><span data-stu-id="725fa-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="725fa-109">Ví dụ: nếu bạn muốn chia sẻ tất cả nội dung của một thư mục, ngoại trừ một tệp trong đó, hãy di chuyển tệp đó sang vị trí mới không được chia sẻ.</span><span class="sxs-lookup"><span data-stu-id="725fa-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="725fa-110">Nếu bạn có hai thư mục con trong một thư mục và bạn muốn chia sẻ một thư mục con với các nhóm A và B và chỉ cho phép một nhóm quyền truy nhập vào thư mục con thứ hai, hãy chia sẻ thư mục mẹ với nhóm A và thêm nhóm B vào thư mục con đầu tiên.</span><span class="sxs-lookup"><span data-stu-id="725fa-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="725fa-111">Dừng chia sẻ tệp hoặc thư mục </span><span class="sxs-lookup"><span data-stu-id="725fa-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

