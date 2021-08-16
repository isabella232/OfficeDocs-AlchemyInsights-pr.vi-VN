---
title: Thuộc tính LỗiValueMustBeUnique
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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002149"
---
# <a name="error-attributevaluemustbeunique"></a>Lỗi: AttributeValueMustBeUnique

Lý do phổ biến nhất cho lỗi AttributeValueMustBeUnique là hai đối tượng có các thuộc tính SourceAnchor (immutableId) khác nhau có cùng giá trị cho các thuộc tính ProxyAddresses và/hoặc UserPrincipalName. Cách khắc phục lỗi AttributeValueMustBeUnique:
  
1. Xác định proxyAddresses trùng lặp, userPrincipalName hoặc giá trị thuộc tính khác đang gây ra lỗi. Ngoài ra, xác định hai (hoặc nhiều) đối tượng liên quan đến xung đột. Báo cáo do Azure AD Kết nối Health tạo để đồng bộ có thể giúp bạn xác định hai đối tượng.
    
2. Xác định đối tượng cần tiếp tục có giá trị trùng lặp và đối tượng nào không nên có.
    
3. Loại bỏ giá trị trùng lặp khỏi đối tượng không nên có giá trị đó. Lưu ý rằng bạn nên thực hiện thay đổi trong thư mục có nguồn gốc của đối tượng. Trong một số trường hợp, bạn có thể cần xóa một trong các đối tượng đang xung đột.
    
4. Nếu bạn đã thực hiện thay đổi trong AD tại chỗ, hãy để Azure AD Kết nối đồng bộ thay đổi để khắc phục lỗi.
    

