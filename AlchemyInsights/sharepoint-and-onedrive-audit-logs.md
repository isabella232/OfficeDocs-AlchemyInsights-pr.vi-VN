---
title: Báo cáo Nhật ký kiểm tra SharePoint cổ điển
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
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662230"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="0fc70-102">Nhật ký kiểm tra SharePoint và OneDrive</span><span class="sxs-lookup"><span data-stu-id="0fc70-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="0fc70-103">Nhật ký kiểm tra cổ điển SharePoint</span><span class="sxs-lookup"><span data-stu-id="0fc70-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="0fc70-104">Mô hình thừa kế của SPO được di chuyển đến Nhật ký kiểm tra hợp nhất (UAL).</span><span class="sxs-lookup"><span data-stu-id="0fc70-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="0fc70-105">Tất cả báo cáo kiểm nghiệm kế thừa của SPO sẽ được hỗ trợ thông qua UAL và các tín hiệu kiểm tra kế thừa đã được di chuyển đến UAL.</span><span class="sxs-lookup"><span data-stu-id="0fc70-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="0fc70-106">Các thay đổi then chốt:</span><span class="sxs-lookup"><span data-stu-id="0fc70-106">Key changes:</span></span>

* <span data-ttu-id="0fc70-107">Dấu cắt không sẵn dùng như một khả năng.</span><span class="sxs-lookup"><span data-stu-id="0fc70-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="0fc70-108">Chọn các sự kiện cụ thể để kiểm nghiệm không sẵn dùng.</span><span class="sxs-lookup"><span data-stu-id="0fc70-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="0fc70-109">Tham khảo [tài liệu này](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) để biết danh sách đầy đủ các sự kiện được kiểm nhập sẵn dùng theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="0fc70-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="0fc70-110">Tùy chọn **vị trí** trong **báo cáo tùy chỉnh** không sẵn dùng.</span><span class="sxs-lookup"><span data-stu-id="0fc70-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="0fc70-111">Tùy chọn **mở hoặc tải xuống** các sự kiện tài liệu không sẵn dùng.</span><span class="sxs-lookup"><span data-stu-id="0fc70-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="0fc70-112">Cấu hình thiết đặt kiểm nghiệm cho tuyển tập trang</span><span class="sxs-lookup"><span data-stu-id="0fc70-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="0fc70-113">Các Nhật ký kiểm tra hợp nhất trong SharePoint và OneDrive hiện đại từ việc tuân thủ</span><span class="sxs-lookup"><span data-stu-id="0fc70-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="0fc70-114">Bật/tắt ghi nhật ký kiểm tra hợp nhất</span><span class="sxs-lookup"><span data-stu-id="0fc70-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="0fc70-115">Không cần cấu hình bổ sung nào trong SharePoint hoặc OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0fc70-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="0fc70-116">Sử dụng tính năng tìm kiếm Nhật ký kiểm tra để kiểm tra hoạt động của (các) tệp, (các) (các) (các) (các) người dùng, quyền:</span><span class="sxs-lookup"><span data-stu-id="0fc70-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="0fc70-117">Các hoạt động của tệp và trang</span><span class="sxs-lookup"><span data-stu-id="0fc70-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="0fc70-118">Hoạt động của thư mục</span><span class="sxs-lookup"><span data-stu-id="0fc70-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="0fc70-119">Các hoạt động yêu cầu chia sẻ và truy nhập</span><span class="sxs-lookup"><span data-stu-id="0fc70-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="0fc70-120">Các hoạt động đồng bộ</span><span class="sxs-lookup"><span data-stu-id="0fc70-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="0fc70-121">Hoạt động quản trị site</span><span class="sxs-lookup"><span data-stu-id="0fc70-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="0fc70-122">Để biết thêm thông tin về cách truy xuất các sự kiện này, hãy xem [Tìm kiếm Nhật ký kiểm](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)tra.</span><span class="sxs-lookup"><span data-stu-id="0fc70-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
