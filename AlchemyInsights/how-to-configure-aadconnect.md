---
title: 646 cách đặt cấu hình cho kết nối
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704511"
---
# <a name="configure-sync-features"></a><span data-ttu-id="473d5-102">Đặt cấu hình các tính năng đồng bộ</span><span class="sxs-lookup"><span data-stu-id="473d5-102">Configure sync features</span></span>

<span data-ttu-id="473d5-103">Azure AD Connect bao gồm một số tính năng được bật theo mặc định, hoặc bạn có thể bật sau này.</span><span class="sxs-lookup"><span data-stu-id="473d5-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="473d5-104">Một số tính năng yêu cầu cấu hình bổ sung trong các môi trường cụ thể.</span><span class="sxs-lookup"><span data-stu-id="473d5-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="473d5-105">[Lọc](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) giới hạn đối tượng được đồng bộ hóa với Azure AD.</span><span class="sxs-lookup"><span data-stu-id="473d5-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="473d5-106">Theo mặc định, tất cả người dùng, liên hệ, nhóm và tài khoản máy tính chạy Windows 10 đều được đồng bộ.</span><span class="sxs-lookup"><span data-stu-id="473d5-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="473d5-107">Bạn có thể bao gồm hoặc loại trừ các đối tượng dựa trên tên miền, dữ hoặc thuộc tính khác.</span><span class="sxs-lookup"><span data-stu-id="473d5-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="473d5-108">[Đồng bộ hóa hash mật khẩu đồng bộ hóa](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) băm mật khẩu từ Active Directory tại chỗ vào Azure AD.</span><span class="sxs-lookup"><span data-stu-id="473d5-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="473d5-109">Điều này cho phép quản lý mật khẩu ở một vị trí, nhưng sử dụng cùng một mật khẩu trong cả môi trường trên nền tảng tại cơ sở và điện toán đám mây.</span><span class="sxs-lookup"><span data-stu-id="473d5-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="473d5-110">Vì Active Directory là nguồn có thẩm quyền, bạn có thể sử dụng chính sách mật khẩu của riêng bạn.</span><span class="sxs-lookup"><span data-stu-id="473d5-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="473d5-111">[Đặt lại mật khẩu tự phục vụ (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) cho phép người dùng đặt lại mật khẩu của riêng mình trong nền tảng điện toán đám mây trong khi vẫn áp dụng chính sách mật khẩu tại cơ sở của bạn.</span><span class="sxs-lookup"><span data-stu-id="473d5-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="473d5-112">[Writeback thiết bị](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) cho phép các thiết bị đã đăng ký trong Azure AD được ghi lại vào Active Directory tại chỗ để chúng có thể sử dụng cho Access có điều kiện.</span><span class="sxs-lookup"><span data-stu-id="473d5-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="473d5-113">[Tránh xóa bỏ tình cờ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) được bật theo mặc định để giúp ngăn không cho quá nhiều đối tượng đồng thời (hơn 500 đối tượng đồng bộ).</span><span class="sxs-lookup"><span data-stu-id="473d5-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="473d5-114">Bạn có thể thay đổi thiết đặt này để đáp ứng nhu cầu của tổ chức của mình.</span><span class="sxs-lookup"><span data-stu-id="473d5-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="473d5-115">Tính năng [nâng cấp tự động](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) được bật theo mặc định cho việc cài đặt hiện tại và giúp đảm bảo Phiên bản của bạn kết nối Azure AD luôn là hiện tại.</span><span class="sxs-lookup"><span data-stu-id="473d5-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
