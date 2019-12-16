---
title: Khắc phục sự cố hiệu suất OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 5416da63851de8b0b45e1d5c0cef24b03db40e6e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054976"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="03448-102">Khắc phục sự cố hiệu suất OneDrive</span><span class="sxs-lookup"><span data-stu-id="03448-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="03448-103">Nếu bạn đang gặp phải đồng bộ chậm hơn mong đợi hoặc các vấn đề hiệu suất tương tự với OneDrive:</span><span class="sxs-lookup"><span data-stu-id="03448-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="03448-104">Xác nhận không có vấn đề đã biết bằng cách sử dụng [bảng điều khiển dịch vụ y tế](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="03448-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="03448-105">[Bật tập tin theo yêu cầu](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) để bạn có thể truy cập tất cả các tệp của mình trong OneDrive mà không cần phải tải xuống tất cả và sử dụng dung lượng bộ nhớ trên thiết bị của mình.</span><span class="sxs-lookup"><span data-stu-id="03448-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="03448-106">[Đánh giá các phương pháp hay nhất](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) về lập kế hoạch và hiệu suất mạng.</span><span class="sxs-lookup"><span data-stu-id="03448-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="03448-107">[Tối đa hóa tốc độ upload và tải xuống](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), đặc biệt nếu bạn đang đồng bộ hoá thiết bị lần đầu tiên.</span><span class="sxs-lookup"><span data-stu-id="03448-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="03448-108">Nếu bạn đang đồng bộ hoá một thư viện với hơn 100.000 mục, Sync OneDrive có vẻ bị kẹt trong một thời gian dài hoặc trạng thái Hiển thị xử lý 0KB xMB. "</span><span class="sxs-lookup"><span data-stu-id="03448-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="03448-109">Tìm hiểu thêm về đồng bộ hóa [hơn 100.000 tệp](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) cũng như [giới hạn 300.000 tệp được hỗ trợ của OneDrive](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="03448-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="03448-110">Khi người dùng vượt quá giới hạn sử dụng, SharePoint Online throttles bất kỳ yêu cầu thêm từ tài khoản người dùng đó trong một thời gian ngắn.</span><span class="sxs-lookup"><span data-stu-id="03448-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="03448-111">Tất cả hành động của người dùng được điều chỉnh trong khi ga có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="03448-111">All user actions are throttled while the throttle is in effect.</span></span>
