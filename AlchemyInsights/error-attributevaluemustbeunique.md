---
title: Lỗi AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813782"
---
# <a name="error-attributevaluemustbeunique"></a>Lỗi: AttributeValueMustBeUnique

Lý do phổ biến nhất đối với lỗi AttributeValueMustBeUnique là hai đối tượng với SourceAnchor khác nhau (Immudtableid) có cùng một giá trị cho ProxyAddresses và/hoặc UserPrincipalName thuộc tính. Để khắc phục lỗi Attributevaluemustbemust:
  
1. Xác định các proxyAddresses trùng lặp, userPrincipalName hoặc giá trị thuộc tính khác gây ra lỗi. Đồng thời, cũng xác định hai đối tượng (hoặc nhiều) liên quan đến cuộc xung đột. Báo cáo được tạo bởi Azure AD Connect Health for Sync có thể giúp bạn xác định hai đối tượng.
    
2. Xác định đối tượng nào nên tiếp tục có giá trị trùng lặp và đối tượng nào không nên làm.
    
3. Loại bỏ giá trị trùng lặp ra khỏi đối tượng không nên có giá trị đó. Lưu ý rằng bạn nên thực hiện thay đổi trong thư mục ở đó đối tượng có nguồn gốc từ đó. Trong một số trường hợp, bạn có thể cần xóa một trong các đối tượng trong xung đột.
    
4. Nếu bạn đã thực hiện thay đổi trong quảng cáo tại cơ sở, hãy để Azure AD kết nối đồng bộ thay đổi cho lỗi để khắc phục.
    

