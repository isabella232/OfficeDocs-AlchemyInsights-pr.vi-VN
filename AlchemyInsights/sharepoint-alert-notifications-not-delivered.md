---
title: Thông báo cảnh báo SharePoint không được chuyển phát
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751265"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="49067-102">Thông báo cảnh báo SharePoint không được chuyển phát</span><span class="sxs-lookup"><span data-stu-id="49067-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="49067-103">Vui lòng kiểm tra thư mục thư rác trong email của bạn, như đôi khi cảnh báo có thể đến đó.</span><span class="sxs-lookup"><span data-stu-id="49067-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="49067-104">Xác định xem **tất cả cảnh báo không được chuyển** phát hay nếu **một cảnh báo riêng lẻ** từ một tệp hoặc thư viện cụ thể không được chuyển phát.</span><span class="sxs-lookup"><span data-stu-id="49067-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="49067-105">**Cảnh báo cá nhân không được chuyển**phát: nếu một cảnh báo riêng lẻ từ một tệp hoặc thư viện cụ thể không được chuyển phát, bạn có thể tìm cách xóa bỏ và tạo lại nó.</span><span class="sxs-lookup"><span data-stu-id="49067-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="49067-106">Xem mục [quản lý, xem hoặc xóa bỏ cảnh báo SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) để tạo lại cảnh báo.</span><span class="sxs-lookup"><span data-stu-id="49067-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="49067-107">**Tất cả cảnh báo không được chuyển**phát: nếu tất cả các cảnh báo từ nhiều tệp hoặc thư viện sẽ không được chuyển phát, hãy truy nhập bảng điều khiển trạng thái [dịch vụ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) để kiểm tra bất kỳ sự cố nào có thể xảy ra với SharePoint hoặc Exchange.</span><span class="sxs-lookup"><span data-stu-id="49067-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="49067-108">Vấn đề có thể với khả năng hoặc sự chậm trễ của SharePoint Alert trong email thông qua Exchange.</span><span class="sxs-lookup"><span data-stu-id="49067-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="49067-109">Điều này cũng sẽ quan trọng cần lưu ý xem email khác đang được chuyển phát và nếu không, vấn đề có thể xảy ra sự chậm trễ của Exchange.</span><span class="sxs-lookup"><span data-stu-id="49067-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="49067-110">Câu hỏi thường gặp về cảnh báo:</span><span class="sxs-lookup"><span data-stu-id="49067-110">FAQ on alerts:</span></span>

- <span data-ttu-id="49067-111">Bạn không thể gửi cảnh báo cho nhóm phân phối, chỉ bảo mật và các nhóm O365 được hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="49067-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="49067-112">Bạn không thể tùy chỉnh các mẫu email cảnh báo; bạn cần sử dụng dòng công việc trình thiết kế Microsoft hoặc SharePoint để đạt được những nội dung đó.</span><span class="sxs-lookup"><span data-stu-id="49067-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

## <a name="related-topics"></a><span data-ttu-id="49067-113">Chủ đề liên quan</span><span class="sxs-lookup"><span data-stu-id="49067-113">Related Topics</span></span>

<span data-ttu-id="49067-114">Bạn muốn thử Microsoft Flow trong SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="49067-114">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="49067-115">Tạo dòng</span><span class="sxs-lookup"><span data-stu-id="49067-115">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="49067-116">SharePoint và dòng</span><span class="sxs-lookup"><span data-stu-id="49067-116">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
