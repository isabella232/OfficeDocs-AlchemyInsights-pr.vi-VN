---
title: Ánh xạ thư viện SharePoint vào ổ đĩa mạng
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 9115a3ab8d1234127a95628a9a49679ef06f6d39
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806205"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="8005e-102">Ánh xạ thư viện SharePoint vào ổ đĩa mạng</span><span class="sxs-lookup"><span data-stu-id="8005e-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="8005e-103">Ánh xạ thư viện dưới dạng ổ đĩa mạng tạm thời và được hỗ trợ chỉ qua Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="8005e-103">Mapping a library as a network drive is temporary and supported only through Internet Explorer.</span></span> <span data-ttu-id="8005e-104">Đôi khi bạn phải mở site SharePoint trong Internet Explorer, rồi chọn duy **trì trạng thái đăng nhập** để ngăn không cho phiên làm việc hết hạn.</span><span class="sxs-lookup"><span data-stu-id="8005e-104">You must occasionally open the SharePoint site in Internet Explorer and select **Stay signed in** to prevent the session from expiring.</span></span> <span data-ttu-id="8005e-105">Thay vào đó, [đồng bộ các tệp SharePoint với máy khách đồng bộ OneDrive mới](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) </a> cung cấp [tệp theo yêu cầu](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span><span class="sxs-lookup"><span data-stu-id="8005e-105">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span> <span data-ttu-id="8005e-106">Truy nhập tất cả các tệp của bạn trong OneDrive mà không sử dụng dung lượng lưu trữ cục bộ.</span><span class="sxs-lookup"><span data-stu-id="8005e-106">Access all your files in OneDrive without using local storage space.</span></span>

<span data-ttu-id="8005e-107">Nếu bạn chọn ánh xạ ổ đĩa thay vì [sử dụng máy khách đồng bộ OneDrive mới](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), hãy đảm bảo bạn làm theo các bước trong bài viết dưới đây.</span><span class="sxs-lookup"><span data-stu-id="8005e-107">If you choose to map a drive instead of [using the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), ensure you follow the steps in the article below.</span></span> 


<span data-ttu-id="8005e-108">**Cách cấu hình và khắc phục sự cố ổ đĩa mạng được ánh xạ**</span><span class="sxs-lookup"><span data-stu-id="8005e-108">**How to configure and troubleshoot mapped network drives**</span></span>


<span data-ttu-id="8005e-109">Xem [khắc phục sự cố các ổ đĩa mạng được ánh xạ kết nối với SharePoint onlines](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="8005e-109">See [Troubleshoot mapped network drives that connect to SharePoint Onlines](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>

<span data-ttu-id="8005e-110">LƯU ý: nếu bạn sử dụng Internet Explorer 10 với Windows 8 hoặc Windows 7 và nhận **quyền truy nhập bị từ chối** hoặc **đường dẫn không thể truy nhập được** khi ánh xạ một ổ đĩa, hãy cài đặt [hotfix này](https://support.microsoft.com/help/2846960) để giải quyết vấn đề này.</span><span class="sxs-lookup"><span data-stu-id="8005e-110">NOTE:  If you use Internet Explorer 10 with Windows 8 or Windows 7, and receive **Access denied** or **Path is not accessible** when mapping a drive, install [this hotfix](https://support.microsoft.com/help/2846960) to resolve this problem.</span></span> 
