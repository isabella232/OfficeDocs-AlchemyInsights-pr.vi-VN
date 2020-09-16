---
title: Khắc phục sự cố hiệu suất của OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757907"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="1e0ce-102">Khắc phục sự cố hiệu suất của OneDrive</span><span class="sxs-lookup"><span data-stu-id="1e0ce-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="1e0ce-103">Nếu bạn đang gặp phải đồng bộ chậm hơn so với dự kiến, hoặc các vấn đề về hiệu suất tương tự với OneDrive:</span><span class="sxs-lookup"><span data-stu-id="1e0ce-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="1e0ce-104">Xác nhận không có vấn đề đã biết bằng cách dùng bảng điều khiển trạng thái [dịch vụ](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="1e0ce-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="1e0ce-105">Cho [phép các tệp theo yêu cầu](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) để bạn có thể truy nhập tất cả các tệp của mình trong OneDrive mà không cần tải xuống tất cả chúng và sử dụng dung lượng lưu trữ trên thiết bị của bạn.</span><span class="sxs-lookup"><span data-stu-id="1e0ce-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="1e0ce-106">[Xem lại các cách thực hành tốt nhất](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) cho việc lập kế hoạch mạng và hiệu suất.</span><span class="sxs-lookup"><span data-stu-id="1e0ce-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="1e0ce-107">[Tối đa hóa tốc độ tải lên và tải xuống](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), đặc biệt là nếu bạn đang đồng bộ một thiết bị lần đầu tiên.</span><span class="sxs-lookup"><span data-stu-id="1e0ce-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="1e0ce-108">Nếu bạn đang đồng bộ một thư viện có nhiều mục hơn 100.000, OneDrive Sync có thể có vẻ khó khăn trong một thời gian dài, hoặc trạng thái Hiển thị xử lý 0KB của xMB. "</span><span class="sxs-lookup"><span data-stu-id="1e0ce-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="1e0ce-109">[Tìm hiểu thêm về cách đồng bộ hóa các tệp 100.000](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) cũng như [giới hạn hỗ trợ của onedrive của các tệp 300.000](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="1e0ce-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="1e0ce-110">Khi người dùng vượt quá giới hạn sử dụng, SharePoint Online sẽ thêm bất kỳ yêu cầu nào từ tài khoản người dùng đó trong một kỳ hạn ngắn.</span><span class="sxs-lookup"><span data-stu-id="1e0ce-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="1e0ce-111">Tất cả các hành động của người dùng đều bị Throttled trong khi có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="1e0ce-111">All user actions are throttled while the throttle is in effect.</span></span>
