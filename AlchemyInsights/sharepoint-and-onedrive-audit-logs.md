---
title: Báo cáo Nhật ký kiểm tra SharePoint cổ điển
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741987"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="be0c7-102">Nhật ký kiểm tra SharePoint và OneDrive</span><span class="sxs-lookup"><span data-stu-id="be0c7-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="be0c7-103">SharePoint cổ điển kiểm tra Nhật ký</span><span class="sxs-lookup"><span data-stu-id="be0c7-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="be0c7-104">Kiểm tra kế thừa SPO được di chuyển sang Nhật ký kiểm tra hợp nhất (UAL).</span><span class="sxs-lookup"><span data-stu-id="be0c7-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="be0c7-105">Tất cả các báo cáo kiểm toán kế thừa SPO sẽ được cung cấp thông qua UAL, và các tín hiệu kiểm toán hợp lệ đã được di chuyển đến UAL.</span><span class="sxs-lookup"><span data-stu-id="be0c7-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="be0c7-106">Thay đổi chính:</span><span class="sxs-lookup"><span data-stu-id="be0c7-106">Key changes:</span></span>

* <span data-ttu-id="be0c7-107">Trimming là không có sẵn như là một khả năng.</span><span class="sxs-lookup"><span data-stu-id="be0c7-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="be0c7-108">Chọn các sự kiện cụ thể để kiểm tra không có sẵn.</span><span class="sxs-lookup"><span data-stu-id="be0c7-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="be0c7-109">Tham khảo [tài liệu này](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) để biết danh sách đầy đủ các sự kiện được kiểm toán có sẵn theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="be0c7-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="be0c7-110">Tùy chọn **vị trí** trong **báo cáo tùy chỉnh** không có sẵn.</span><span class="sxs-lookup"><span data-stu-id="be0c7-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="be0c7-111">Tùy chọn **mở hoặc tải xuống** các sự kiện tài liệu không khả dụng.</span><span class="sxs-lookup"><span data-stu-id="be0c7-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="be0c7-112">Cấu hình thiết đặt kiểm tra cho bộ sưu tập trang web</span><span class="sxs-lookup"><span data-stu-id="be0c7-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="be0c7-113">SharePoint và OneDrive hiện đại thống nhất kiểm tra Nhật ký từ tuân thủ</span><span class="sxs-lookup"><span data-stu-id="be0c7-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="be0c7-114">Bật/tắt ghi nhật ký kiểm tra hợp nhất</span><span class="sxs-lookup"><span data-stu-id="be0c7-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="be0c7-115">Không có cấu hình bổ sung được yêu cầu trong SharePoint hoặc OneDrive.</span><span class="sxs-lookup"><span data-stu-id="be0c7-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="be0c7-116">Sử dụng kiểm tra ghi nhật ký tìm kiếm để kiểm tra hoạt động của tệp (s), cặp (s), người dùng (s), quyền:</span><span class="sxs-lookup"><span data-stu-id="be0c7-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="be0c7-117">Hoạt động tập tin và trang</span><span class="sxs-lookup"><span data-stu-id="be0c7-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="be0c7-118">Hoạt động thư mục</span><span class="sxs-lookup"><span data-stu-id="be0c7-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="be0c7-119">Chia sẻ và truy cập các hoạt động yêu cầu</span><span class="sxs-lookup"><span data-stu-id="be0c7-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="be0c7-120">Hoạt động đồng bộ hóa</span><span class="sxs-lookup"><span data-stu-id="be0c7-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="be0c7-121">Hoạt động quản trị trang web</span><span class="sxs-lookup"><span data-stu-id="be0c7-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="be0c7-122">Để biết thêm thông tin về cách lấy các sự kiện, [hãy xem tìm kiếm Nhật ký kiểm tra](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="be0c7-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
