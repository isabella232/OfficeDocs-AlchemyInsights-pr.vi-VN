---
title: ConsistencyGuid / sourceAnchor hành vi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517017"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="9a910-102">ConsistencyGuid / sourceAnchor hành vi</span><span class="sxs-lookup"><span data-stu-id="9a910-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="9a910-103">Azure quảng cáo kết nối (Phiên bản 1.1.524.0 và sau) bây giờ tạo điều kiện sử dụng msDS-ConsistencyGuid như là thuộc tính sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="9a910-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="9a910-104">Khi sử dụng tính năng này, Azure quảng cáo kết nối tự động cấu hình các quy tắc đồng bộ hóa cho:</span><span class="sxs-lookup"><span data-stu-id="9a910-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="9a910-105">Sử dụng msDS-ConsistencyGuid như là thuộc tính sourceAnchor cho đối tượng người dùng.</span><span class="sxs-lookup"><span data-stu-id="9a910-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="9a910-106">ObjectGUID được sử dụng cho các loại đối tượng khác.</span><span class="sxs-lookup"><span data-stu-id="9a910-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="9a910-107">Đối với bất kỳ cung cấp tại chỗ quảng cáo dùng đối tượng có thuộc tính msDS-ConsistencyGuid không phải là dân cư, Azure quảng cáo kết nối viết các giá trị objectGUID lại cho thuộc tính msDS ConsistencyGuid trong Active Directory tại chỗ.</span><span class="sxs-lookup"><span data-stu-id="9a910-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="9a910-108">Sau khi các thuộc tính msDS-ConsistencyGuid dân cư đông đúc, Azure quảng cáo kết nối sau đó xuất khẩu các đối tượng để quảng cáo Azure.</span><span class="sxs-lookup"><span data-stu-id="9a910-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="9a910-109">**Lưu ý:** Một khi một chỗ đối tượng quảng cáo nhập khẩu vào Azure quảng cáo kết nối (có nghĩa là, được nhập vào không gian kết nối AD và dự kiến vào Metaverse), bạn không thể thay đổi giá trị sourceAnchor của nó nữa.</span><span class="sxs-lookup"><span data-stu-id="9a910-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="9a910-110">Để xác định giá trị sourceAnchor cho một cho tại chỗ quảng cáo đối tượng, cấu hình thuộc tính msDS-ConsistencyGuid của nó trước khi nó được nhập vào Azure quảng cáo kết nối.</span><span class="sxs-lookup"><span data-stu-id="9a910-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="9a910-111">Để biết thêm chi tiết về SourceAnchor và ConsistencyGuid, tham khảo như sau: [Azure quảng cáo kết nối: thiết kế khái niệm](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="9a910-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

