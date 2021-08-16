---
title: Hạn chế truy nhập trong SharePoint hoặc OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075062"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Hạn chế truy nhập trong SharePoint hoặc OneDrive

Trong SharePoint và OneDrive, bạn hạn chế quyền truy nhập vào các mục như tệp, thư mục và danh sách bằng cách chỉ cấp quyền truy nhập cho các nhóm hoặc cá nhân mà bạn muốn có quyền truy nhập. Theo mặc định, các quyền SharePoint được thừa kế từ cao hơn lên trong cấu trúc phân cấp. Vì vậy, một tệp kế thừa quyền của nó từ thư mục kế thừa quyền của nó từ thư viện, kế thừa quyền của nó từ site.
  
Bạn có thể chia sẻ ở mức cao hơn (chẳng hạn như bằng cách chia sẻ toàn bộ site) và sau đó ngắt kế thừa nếu bạn không muốn chia sẻ tất cả các mục trên site. Tuy nhiên, chúng tôi không đề xuất điều này vì nó làm cho việc duy trì các quyền phức tạp hơn và gây nhầm lẫn trong tương lai. Thay vào đó, bạn có thể thực hiện điều này:
  
- Ví dụ: nếu bạn muốn chia sẻ tất cả nội dung của một thư mục ngoại trừ một tệp trong đó, hãy di chuyển tệp đó đến vị trí mới không được chia sẻ.
    
- Nếu bạn có hai thư mục con trong một thư mục và bạn muốn chia sẻ một thư mục con với các nhóm A và B và chỉ cho phép truy nhập vào thư mục con thứ hai của nhóm A, hãy chia sẻ thư mục mẹ với nhóm A và thêm nhóm B vào thư mục con đầu tiên.
    
[Ngừng chia sẻ tệp hoặc thư mục ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

