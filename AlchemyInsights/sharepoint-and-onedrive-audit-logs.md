---
title: Báo cáo Nhật ký kiểm tra SharePoint cổ điển
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068045"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="6ed22-102">Nhật ký kiểm tra SharePoint và OneDrive</span><span class="sxs-lookup"><span data-stu-id="6ed22-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="6ed22-103">**SharePoint và OneDrive hiện đại thống nhất kiểm tra Nhật ký từ tuân thủ**</span><span class="sxs-lookup"><span data-stu-id="6ed22-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="6ed22-104">Bật/tắt ghi nhật ký kiểm tra hợp nhất</span><span class="sxs-lookup"><span data-stu-id="6ed22-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="6ed22-105">Không có cấu hình bổ sung được yêu cầu trong SharePoint hoặc OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6ed22-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="6ed22-106">Sử dụng kiểm tra ghi nhật ký tìm kiếm để kiểm tra hoạt động của tệp (s), cặp (s), người dùng (s), quyền:</span><span class="sxs-lookup"><span data-stu-id="6ed22-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="6ed22-107">Hoạt động tập tin và trang</span><span class="sxs-lookup"><span data-stu-id="6ed22-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="6ed22-108">Hoạt động thư mục</span><span class="sxs-lookup"><span data-stu-id="6ed22-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="6ed22-109">Chia sẻ và truy cập các hoạt động yêu cầu</span><span class="sxs-lookup"><span data-stu-id="6ed22-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="6ed22-110">Hoạt động đồng bộ hóa</span><span class="sxs-lookup"><span data-stu-id="6ed22-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="6ed22-111">Hoạt động quản trị trang web</span><span class="sxs-lookup"><span data-stu-id="6ed22-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="6ed22-112">Để biết thêm thông tin về cách lấy các sự kiện, [hãy xem tìm kiếm Nhật ký kiểm tra](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="6ed22-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="6ed22-113">**SharePoint cổ điển kiểm tra Nhật ký**</span><span class="sxs-lookup"><span data-stu-id="6ed22-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="6ed22-114">Chúng tôi đã di chuyển SPO kế thừa kiểm toán hợp nhất kiểm tra đăng nhập (UAL).</span><span class="sxs-lookup"><span data-stu-id="6ed22-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="6ed22-115">Điều này về cơ bản có nghĩa là tất cả các báo cáo kiểm toán hợp lệ SPO bây giờ sẽ được cung cấp thông qua UAL, và các tín hiệu kiểm toán hợp lệ đã được di chuyển đến UAL.</span><span class="sxs-lookup"><span data-stu-id="6ed22-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="6ed22-116">Thay đổi chính:</span><span class="sxs-lookup"><span data-stu-id="6ed22-116">Key changes:</span></span>

- <span data-ttu-id="6ed22-117">Trimming như là một khả năng không có sẵn.</span><span class="sxs-lookup"><span data-stu-id="6ed22-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="6ed22-118">Phần mà bạn chọn các sự kiện cụ thể để kiểm tra là không có sẵn.</span><span class="sxs-lookup"><span data-stu-id="6ed22-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="6ed22-119">Vui lòng tham khảo [tài liệu này](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) để biết danh sách đầy đủ các sự kiện được kiểm toán có sẵn theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="6ed22-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="6ed22-120">Tuỳ chọn "vị trí" trong **báo cáo tuỳ chỉnh** không khả dụng.</span><span class="sxs-lookup"><span data-stu-id="6ed22-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="6ed22-121">Sự kiện "mở hoặc tải xuống tài liệu" không khả dụng.</span><span class="sxs-lookup"><span data-stu-id="6ed22-121">“Opening or downloading documents” events is NOT available.</span></span> 

