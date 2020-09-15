---
title: Sự cố khi mở hoặc tải xuống các tệp trong yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695671"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="c0e46-102">Sự cố khi mở hoặc tải xuống các tệp trong yammer</span><span class="sxs-lookup"><span data-stu-id="c0e46-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="c0e46-103">Yammer cổ điển hỗ trợ nhiều tùy chọn để tải lên tệp tin nhắn và nhóm.</span><span class="sxs-lookup"><span data-stu-id="c0e46-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="c0e46-104">Tùy thuộc vào cấu hình mạng, các tệp mặc định là lưu trữ trong SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c0e46-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="c0e46-105">Bộ chọn tệp trong mới yammer vẫn chưa hỗ trợ tất cả các tùy chọn sẵn dùng trong yammer cổ điển.</span><span class="sxs-lookup"><span data-stu-id="c0e46-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="c0e46-106">Bản Cập Nhật trong tương lai sẽ thêm các tính năng bổ sung.</span><span class="sxs-lookup"><span data-stu-id="c0e46-106">A future update will add additional features.</span></span> <span data-ttu-id="c0e46-107">Để biết thêm thông tin, hãy xem [đính kèm tệp hoặc hình ảnh vào bài đăng hội thoại yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="c0e46-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="c0e46-108">**Không thể mở hoặc tải xuống tệp**</span><span class="sxs-lookup"><span data-stu-id="c0e46-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="c0e46-109">Một tệp có thể tải lên yammer mà còn được liên kết đến một tệp trong SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="c0e46-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="c0e46-110">Để khắc phục sự cố, trước tiên, bạn phải xác định vị trí của tệp.</span><span class="sxs-lookup"><span data-stu-id="c0e46-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="c0e46-111">Nếu tệp đã được tải lên yammer, nó sẽ có URL \*. yammer.com.</span><span class="sxs-lookup"><span data-stu-id="c0e46-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="c0e46-112">Đảm bảo rằng các URL và địa chỉ IP được yêu cầu không bị chặn.</span><span class="sxs-lookup"><span data-stu-id="c0e46-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="c0e46-113">Để biết thêm thông tin, hãy xem bài đăng blog [bằng địa chỉ IP được mã hóa cứng cho yammer không được đề](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)xuất.</span><span class="sxs-lookup"><span data-stu-id="c0e46-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="c0e46-114">Kiểm tra xem người dùng cũng là người quản trị toàn cầu có thể tải xuống tệp hay không.</span><span class="sxs-lookup"><span data-stu-id="c0e46-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="c0e46-115">Nếu tệp là riêng tư, bạn có thể phải sử dụng chế độ nội dung riêng tư.</span><span class="sxs-lookup"><span data-stu-id="c0e46-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="c0e46-116">Để biết thêm thông tin, hãy xem sau đó [giám sát nội dung riêng tư trong yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="c0e46-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="c0e46-117">**Các khách hàng và các tệp cấp độ mạng yammer trong SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="c0e46-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="c0e46-118">Các [khách hàng ở mức mạng trong yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) không sử dụng AZURE AD B2B và nằm bên trong dịch vụ yammer, vì vậy họ không thể truy nhập các tệp yammer được lưu trữ trong SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c0e46-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="c0e46-119">Tạo một người dùng B2B bên ngoài người dùng có thể truy nhập vào thư viện tài liệu trong SharePoint Online bằng cách sử dụng danh tính đó.</span><span class="sxs-lookup"><span data-stu-id="c0e46-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="c0e46-120">Để biết thông tin về việc tương lai Azure AD B2B hỗ trợ khách trong yammer, hãy xem [hỗ trợ khách mời Business-to-Business (B2B) trong bản xem trước yammer-các điều khoản và câu hỏi thường gặp của khách hàng](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="c0e46-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>