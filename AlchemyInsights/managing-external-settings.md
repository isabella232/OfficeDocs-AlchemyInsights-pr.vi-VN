---
title: Quản lý thiết đặt bên ngoài
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294428"
---
# <a name="managing-external-settings"></a><span data-ttu-id="84152-102">Quản lý thiết đặt bên ngoài</span><span class="sxs-lookup"><span data-stu-id="84152-102">Managing External Settings</span></span>

<span data-ttu-id="84152-103">**Thông báo**</span><span class="sxs-lookup"><span data-stu-id="84152-103">**Announcement**</span></span>

- <span data-ttu-id="84152-104">[Deprecation của WebView hỗ trợ đăng nhập từ Google bắt đầu từ 4 tháng 1, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span><span class="sxs-lookup"><span data-stu-id="84152-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="84152-105">Kiểm tra xem ứng dụng của bạn có bị ảnh hưởng bằng cách theo dõi hướng dẫn của Google trên tính tương thích kiểm tra không</span><span class="sxs-lookup"><span data-stu-id="84152-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="84152-106">Đảm bảo sử dụng WebView System hoặc trình duyệt hệ thống khi đăng nhập vào người dùng của bạn với tài khoản Google dành cho người dùng</span><span class="sxs-lookup"><span data-stu-id="84152-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="84152-107">**Quản lý thiết đặt lời mời**</span><span class="sxs-lookup"><span data-stu-id="84152-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="84152-108">Xác nhận rằng bạn đã [cấu hình các thiết đặt cộng tác bên ngoài](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) để cho phép những người thích hợp gửi thư mời.</span><span class="sxs-lookup"><span data-stu-id="84152-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="84152-109">**Quản lý quyền truy nhập của người dùng khách**</span><span class="sxs-lookup"><span data-stu-id="84152-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="84152-110">Người quản trị toàn cầu có thể quản lý quyền truy nhập của khách trong thư mục qua cổng thông tin Azure bằng cách cấu hình quyền truy nhập của khách trên trang thiết đặt cộng tác bên ngoài.</span><span class="sxs-lookup"><span data-stu-id="84152-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="84152-111">[Tìm hiểu thêm về thiết đặt này](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="84152-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="84152-112">Nếu bạn muốn khách của mình truy nhập vào các ứng dụng như nhóm hoặc SharePoint, hãy xác nhận rằng bạn đã cấu hình những ứng dụng này để cho phép truy nhập của khách.</span><span class="sxs-lookup"><span data-stu-id="84152-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="84152-113">Tìm hiểu thêm về các [thiết đặt nhóm](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) và [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="84152-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="84152-114">**Cấu hình thư mời:**</span><span class="sxs-lookup"><span data-stu-id="84152-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="84152-115">Bật cộng tác bên ngoài B2B và quản lý những người có thể mời khách</span><span class="sxs-lookup"><span data-stu-id="84152-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="84152-116">Cho phép hoặc chặn thư mời cho người dùng từ các tổ chức cụ thể</span><span class="sxs-lookup"><span data-stu-id="84152-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="84152-117">**Cấu hình các nhà cung cấp căn cước được phép:**</span><span class="sxs-lookup"><span data-stu-id="84152-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="84152-118">Liên kết Google</span><span class="sxs-lookup"><span data-stu-id="84152-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="84152-119">Liên kết trực tiếp</span><span class="sxs-lookup"><span data-stu-id="84152-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="84152-120">Xác thực mật mã một lần email</span><span class="sxs-lookup"><span data-stu-id="84152-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
