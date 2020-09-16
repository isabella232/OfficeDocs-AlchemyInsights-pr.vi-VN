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
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Hạn chế quyền truy nhập trong SharePoint hoặc OneDrive

Trong SharePoint và OneDrive, bạn hạn chế quyền truy nhập vào các mục như tệp, thư mục và danh sách bằng cách cấp quyền truy nhập chỉ cho các nhóm hoặc cá nhân mà bạn muốn có quyền truy nhập. Theo mặc định, các quyền trong SharePoint được kế thừa từ cao hơn trong cấu trúc phân cấp. Vì vậy, một tệp đã thừa kế quyền của nó từ thư mục, vốn thừa kế quyền của nó từ thư viện, vốn sẽ thừa kế quyền của nó từ site đó.
  
Bạn có thể chia sẻ ở mức cao hơn (chẳng hạn như bằng cách chia sẻ toàn bộ trang) và sau đó ngắt kế thừa nếu bạn không muốn chia sẻ tất cả các mục trên trang web. Tuy nhiên, chúng tôi không khuyên bạn nên điều này vì việc duy trì quyền phức tạp hơn và khó hiểu hơn trong tương lai. Sau đây là những gì bạn có thể thực hiện thay thế:
  
- Ví dụ: nếu bạn muốn chia sẻ tất cả nội dung của một thư mục, ngoại trừ một tệp trong đó, hãy di chuyển tệp đó sang vị trí mới không được chia sẻ.
    
- Nếu bạn có hai thư mục con trong một thư mục và bạn muốn chia sẻ một thư mục con với các nhóm A và B và chỉ cho phép một nhóm quyền truy nhập vào thư mục con thứ hai, hãy chia sẻ thư mục mẹ với nhóm A và thêm nhóm B vào thư mục con đầu tiên.
    
[Dừng chia sẻ tệp hoặc thư mục ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

