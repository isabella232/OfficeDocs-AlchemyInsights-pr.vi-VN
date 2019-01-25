---
title: 646 làm thế nào để cấu hình AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499692"
---
# <a name="configure-sync-features"></a><span data-ttu-id="80110-102">Cấu hình tính năng đồng bộ hóa</span><span class="sxs-lookup"><span data-stu-id="80110-102">Configure sync features</span></span>

<span data-ttu-id="80110-p101">Azure quảng cáo kết nối bao gồm một số tính năng đó được kích hoạt theo mặc định, hoặc bạn có thể kích hoạt sau đó. Một số tính năng yêu cầu cấu hình bổ sung trong môi trường cụ thể.</span><span class="sxs-lookup"><span data-stu-id="80110-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="80110-p102">Giới hạn [lọc](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) các đối tượng được đồng bộ hoá Azure quảng cáo. Theo mặc định, tất cả người dùng, số liên lạc, nhóm, và Windows 10 máy tính tài khoản được đồng bộ hoá. Bạn có thể bao gồm hoặc loại trừ các đối tượng dựa trên tên miền, Anh hoặc thuộc tính khác.</span><span class="sxs-lookup"><span data-stu-id="80110-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="80110-p103">[Mật khẩu băm syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) đồng bộ hóa các hash mật khẩu từ Active Directory tại chỗ để quảng cáo Azure. Điều này cho phép quản lý mật khẩu ở một vị trí, nhưng sử dụng cùng một mật khẩu trong cả hai chỗ mây và môi trường. Vì hoạt động thư mục nguồn thẩm quyền, bạn có thể sử dụng chính sách mật khẩu của riêng bạn.</span><span class="sxs-lookup"><span data-stu-id="80110-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="80110-111">[Đặt lại mật khẩu tự phục vụ (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) cho phép người dùng đặt lại mật khẩu của riêng của họ trong các đám mây trong khi vẫn còn áp dụng chính sách mật khẩu tại chỗ của bạn.</span><span class="sxs-lookup"><span data-stu-id="80110-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="80110-112">[Thiết bị writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) cho phép đăng ký các thiết bị trong các quảng cáo Azure được viết lại để Active Directory tại chỗ để họ có thể được sử dụng để truy cập có điều kiện.</span><span class="sxs-lookup"><span data-stu-id="80110-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="80110-p104">[Ngăn chặn tình cờ xóa](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) được kích hoạt theo mặc định để giúp ngăn chặn quá nhiều đối tượng đồng thời xoá (hơn 500 đối tượng cho một đồng bộ hoá). Bạn có thể thay đổi cài đặt này để đáp ứng nhu cầu của tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="80110-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="80110-115">[Nâng cấp tự động](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) được kích hoạt theo mặc định cho việc cài đặt nhận và giúp đảm bảo rằng các phiên bản của Azure quảng cáo kết nối luôn luôn là hiện tại.</span><span class="sxs-lookup"><span data-stu-id="80110-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

