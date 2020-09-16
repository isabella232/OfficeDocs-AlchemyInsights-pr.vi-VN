---
title: Hành vi Cyguid/Sourceneo nhất quán
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756305"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="3c8c8-102">Hành vi Cyguid/Sourceneo nhất quán</span><span class="sxs-lookup"><span data-stu-id="3c8c8-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="3c8c8-103">Azure AD Connect (Phiên bản 1.1.524.0 và sau) bây giờ tạo điều kiện sử dụng các Cyguid gắn kết với tên thuộc tính sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="3c8c8-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="3c8c8-104">Khi sử dụng tính năng này, Azure AD kết nối sẽ tự động cấu hình các quy tắc đồng bộ hóa để:</span><span class="sxs-lookup"><span data-stu-id="3c8c8-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="3c8c8-105">Sử dụng msDS-chỗ phân vị là thuộc tính sourceAnchor cho đối tượng người dùng.</span><span class="sxs-lookup"><span data-stu-id="3c8c8-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="3c8c8-106">ObjectGUID được dùng cho các kiểu đối tượng khác.</span><span class="sxs-lookup"><span data-stu-id="3c8c8-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="3c8c8-107">Đối với bất kỳ đối tượng người dùng quảng cáo tại cơ sở nào có thuộc tính Cyds-mâu thuẫn không có hàm, Azure AD kết nối sẽ viết giá trị objectGUID của nó trở về thuộc tính Cyguid nhất quán trong Active Directory tại chỗ.</span><span class="sxs-lookup"><span data-stu-id="3c8c8-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="3c8c8-108">Sau đó thuộc tính Cyds-mâu thuẫn, hãy kết nối Azure AD sau đó xuất ra đối tượng Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3c8c8-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="3c8c8-109">**Lưu ý:** Sau khi đối tượng quảng cáo tại cơ sở được nhập vào Azure AD Connect (tức là, được nhập vào không gian kết nối quảng cáo và dự kiến vào metaverse), bạn không thể thay đổi giá trị Sourceneo của nó nữa.</span><span class="sxs-lookup"><span data-stu-id="3c8c8-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="3c8c8-110">Để xác định giá trị sourceAnchor cho đối tượng quảng cáo tại cơ sở đã cho, hãy đặt cấu hình thuộc tính người dùng đồng bộ của msDS trước khi nó được nhập vào Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="3c8c8-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="3c8c8-111">Để biết thêm thông tin về phần giới thiệu về SourceAnchor và mâu thuẫn, hãy tham khảo các thao tác sau: [AZURE AD Connect: khái niệm thiết kế](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="3c8c8-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

