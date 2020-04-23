---
title: 646 làm thế nào để cấu hình AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722588"
---
# <a name="configure-sync-features"></a><span data-ttu-id="60021-102">Cấu hình tính năng đồng bộ</span><span class="sxs-lookup"><span data-stu-id="60021-102">Configure sync features</span></span>

<span data-ttu-id="60021-103">Azure AD kết nối bao gồm một số tính năng được kích hoạt theo mặc định, hoặc bạn có thể kích hoạt sau.</span><span class="sxs-lookup"><span data-stu-id="60021-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="60021-104">Một số tính năng yêu cầu cấu hình bổ sung trong môi trường cụ thể.</span><span class="sxs-lookup"><span data-stu-id="60021-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="60021-105">[Lọc](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) giới hạn các đối tượng được đồng bộ hoá Azure AD.</span><span class="sxs-lookup"><span data-stu-id="60021-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="60021-106">Theo mặc định, tất cả người dùng, danh bạ, nhóm và tài khoản máy tính Windows 10 được đồng bộ hoá.</span><span class="sxs-lookup"><span data-stu-id="60021-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="60021-107">Bạn có thể bao gồm hoặc loại trừ các đối tượng dựa trên miền, OUs hoặc các thuộc tính khác.</span><span class="sxs-lookup"><span data-stu-id="60021-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="60021-108">[Mật khẩu băm đồng bộ hóa](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) mật khẩu băm từ Active Directory tại chỗ sang Azure AD.</span><span class="sxs-lookup"><span data-stu-id="60021-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="60021-109">Điều này cho phép quản lý mật khẩu tại một địa chỉ, nhưng sử dụng cùng một mật khẩu trong môi trường tại chỗ và đám mây.</span><span class="sxs-lookup"><span data-stu-id="60021-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="60021-110">Vì Active Directory là nguồn có thẩm quyền, bạn có thể sử dụng chính sách mật khẩu của riêng bạn.</span><span class="sxs-lookup"><span data-stu-id="60021-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="60021-111">[Tự dịch vụ đặt lại mật khẩu (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) cho phép người dùng đặt lại mật khẩu của riêng mình trong đám mây trong khi vẫn áp dụng chính sách mật khẩu tại chỗ của bạn.</span><span class="sxs-lookup"><span data-stu-id="60021-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="60021-112">[Thiết bị](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) ghi lại cho phép các thiết bị đăng ký trong Azure AD được viết trở lại Active Directory tại chỗ để họ có thể được sử dụng để truy cập có điều kiện.</span><span class="sxs-lookup"><span data-stu-id="60021-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="60021-113">[Ngăn chặn tình cờ xóa](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) được kích hoạt theo mặc định để giúp ngăn chặn quá nhiều xoá đối tượng đồng thời (hơn 500 đối tượng cho mỗi đồng bộ hóa).</span><span class="sxs-lookup"><span data-stu-id="60021-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="60021-114">Bạn có thể thay đổi cài đặt này để đáp ứng nhu cầu của tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="60021-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="60021-115">[Tự động nâng cấp](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) được bật theo mặc định cho các cài đặt nhanh và giúp đảm bảo Phiên bản Azure AD kết nối luôn là hiện tại.</span><span class="sxs-lookup"><span data-stu-id="60021-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
