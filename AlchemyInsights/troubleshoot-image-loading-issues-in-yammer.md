---
title: Khắc phục sự cố tải hình ảnh trong yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148421"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="14474-102">Khắc phục sự cố tải hình ảnh trong yammer</span><span class="sxs-lookup"><span data-stu-id="14474-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="14474-103">Khi sự cố xảy ra với hình ảnh và tệp xem trước trong yammer, khắc phục sự cố bằng cách kiểm tra xem vấn đề xảy ra cho tất cả người dùng, cho dù nó xảy ra trên thiết bị di động, và nếu nó có khả năng tái sản xuất khi tải lên tệp đính kèm.</span><span class="sxs-lookup"><span data-stu-id="14474-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="14474-104">**Vấn đề ảnh hồ sơ**</span><span class="sxs-lookup"><span data-stu-id="14474-104">**Profile photo issues**</span></span>  

<span data-ttu-id="14474-105">Nếu người dùng cuối đăng nhập vào yammer qua Microsoft 365, họ phải thay đổi hồ sơ của họ, bao gồm cả ảnh hồ sơ của họ.</span><span class="sxs-lookup"><span data-stu-id="14474-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="14474-106">Nếu người dùng không được phép thực hiện cập nhật hồ sơ, quản trị viên có thể thực hiện Cập Nhật cho người dùng.</span><span class="sxs-lookup"><span data-stu-id="14474-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="14474-107">Để biết thêm thông tin, hãy xem [xem và cập nhật hồ sơ của bạn trong Office delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="14474-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="14474-108">Để biết thông tin về chỉnh sửa hồ sơ, bao gồm ảnh hồ sơ, xem [thay đổi cài đặt và hồ sơ yammer của tôi](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="14474-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="14474-109">Ảnh hồ sơ Cập Nhật được đồng bộ hóa khác với thuộc tính hồ sơ.</span><span class="sxs-lookup"><span data-stu-id="14474-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="14474-110">Người dùng phải đăng nhập để bắt đầu đồng bộ hóa ảnh hồ sơ của họ.</span><span class="sxs-lookup"><span data-stu-id="14474-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="14474-111">Để biết thông tin, xem [hình ảnh hồ sơ người dùng được Cập Nhật từ Office 365 sang yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="14474-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="14474-112">Để biết thông tin về vòng đời của người dùng cho yammer, hãy xem [quản lý người dùng yammer trên vòng đời của họ từ Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="14474-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="14474-113">Để biết chi tiết về cách đồng bộ hóa ảnh hồ sơ hoạt động trong Microsoft 365, xem [thông tin về đồng bộ hóa ảnh hồ sơ trong microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="14474-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="14474-114">**Xem trước tài liệu và vấn đề hình thu nhỏ**</span><span class="sxs-lookup"><span data-stu-id="14474-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="14474-115">Khi tệp hoặc hình ảnh được đăng lên yammer, xem trước có thể không xuất hiện vì:</span><span class="sxs-lookup"><span data-stu-id="14474-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="14474-116">Tệp bị hỏng và không thể xử lý.</span><span class="sxs-lookup"><span data-stu-id="14474-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="14474-117">Tệp không được gần đây tải lên SharePoint trực tuyến hoặc yammer có siêu dữ liệu không hợp lệ vì các lý do khác.</span><span class="sxs-lookup"><span data-stu-id="14474-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="14474-118">Các URL cần thiết để tải hình ảnh xem trước bị chặn.</span><span class="sxs-lookup"><span data-stu-id="14474-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="14474-119">Bản xem trước tệp đã bị người dùng xóa trước khi đăng.</span><span class="sxs-lookup"><span data-stu-id="14474-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="14474-120">Sự cố dịch vụ ngăn xem trước được tạo ra.</span><span class="sxs-lookup"><span data-stu-id="14474-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="14474-121">**Lưu ý** Xem trước cho các liên kết và tập tin tải lên có thể hành xử khác nhau.</span><span class="sxs-lookup"><span data-stu-id="14474-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="14474-122">Liên kết đến các tệp trên Internet hoặc liên kết yêu cầu xác thực bổ sung có thể không hiển thị đúng.</span><span class="sxs-lookup"><span data-stu-id="14474-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="14474-123">Để biết thêm thông tin, xem [đính kèm tệp hoặc hình ảnh vào thư yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="14474-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 