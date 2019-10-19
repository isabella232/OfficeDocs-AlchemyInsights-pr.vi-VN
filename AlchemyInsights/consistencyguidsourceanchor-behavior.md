---
title: Hành vi của các mâu thuẫn/sourceAnchor
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36517017"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="4223d-102">Hành vi của các mâu thuẫn/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="4223d-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="4223d-103">Azure AD kết nối (Phiên bản 1.1.524.0 và sau) bây giờ tạo điều kiện cho việc sử dụng msDS, Cyguid là sourceAnchor thuộc tính.</span><span class="sxs-lookup"><span data-stu-id="4223d-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="4223d-104">Khi sử dụng tính năng này, Azure AD kết nối tự động cấu hình các quy tắc đồng bộ hóa để:</span><span class="sxs-lookup"><span data-stu-id="4223d-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="4223d-105">Sử dụng msDS sự nhất quán Cyguid là thuộc tính sourceAnchor đối tượng người dùng.</span><span class="sxs-lookup"><span data-stu-id="4223d-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="4223d-106">ObjectGUID được sử dụng cho các loại đối tượng.</span><span class="sxs-lookup"><span data-stu-id="4223d-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="4223d-107">Đối tượng cho bất kỳ chỗ AD người dùng trên cơ sở có msDS-sự nhất quán thuộc tính không được xác định, Azure AD kết nối ghi giá trị objectGUID về thuộc tính msDS-sự nhất quán trong Active Directory tại chỗ.</span><span class="sxs-lookup"><span data-stu-id="4223d-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="4223d-108">Sau khi msDS-thuộc tính chính xác Cyguid được điền, Azure AD kết nối sau đó xuất đối tượng Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4223d-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="4223d-109">**Lưu ý:** Khi một đối tượng AD tại chỗ được nhập vào Azure AD kết nối (tức là, nhập vào không gian kết nối quảng cáo và dự kiến vào metaverse), bạn không thể thay đổi giá trị sourceAnchor nữa.</span><span class="sxs-lookup"><span data-stu-id="4223d-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="4223d-110">Để xác định giá trị sourceAnchor cho một đối tượng quảng cáo tại chỗ, cấu hình thuộc tính msDS của các Cyguid trước khi nó được nhập vào Azure AD kết nối.</span><span class="sxs-lookup"><span data-stu-id="4223d-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="4223d-111">Để biết thêm thông tin về SourceAnchor và sự nhất quán Cyguid, hãy tham khảo sau: [AZURE AD kết nối: thiết kế khái niệm](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="4223d-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

