---
title: Truy nhập bị từ chối khi ánh xạ ổ đĩa sang SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668765"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="7a0e7-102">Khắc phục các vấn đề với thư viện SharePoint được ánh xạ vào ổ đĩa mạng</span><span class="sxs-lookup"><span data-stu-id="7a0e7-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="7a0e7-103">Khi bạn duyệt đến ổ đĩa mạng được ánh xạ, bạn có thể thấy một trong các thông báo sau:</span><span class="sxs-lookup"><span data-stu-id="7a0e7-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="7a0e7-104">**\\Không thể truy nhập được đường dẫn. Có thể bạn không có quyền sử dụng tài nguyên mạng này. Liên hệ với người quản trị của máy chủ này để tìm hiểu xem bạn có quyền truy nhập hay không.**</span><span class="sxs-lookup"><span data-stu-id="7a0e7-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="7a0e7-105">**Truy nhập bị từ chối. Trước khi mở tệp ở vị trí này, trước tiên bạn phải thêm site web vào danh sách site tin cậy của bạn, duyệt đến trang web, rồi chọn tùy chọn để tự động đăng nhập.**</span><span class="sxs-lookup"><span data-stu-id="7a0e7-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="7a0e7-106">[Nhận trợ giúp khắc phục sự cố ổ đĩa mạng được ánh xạ](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="7a0e7-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="7a0e7-107">Ánh xạ thư viện dưới dạng ổ đĩa mạng tạm thời và được hỗ trợ trong Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="7a0e7-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="7a0e7-108">Thay vào đó, [đồng bộ các tệp SharePoint với máy khách đồng bộ OneDrive mới](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) , bao gồm các [tệp theo yêu cầu](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="7a0e7-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="7a0e7-109">Truy nhập tất cả các tệp của bạn trong OneDrive mà không sử dụng dung lượng lưu trữ cục bộ.</span><span class="sxs-lookup"><span data-stu-id="7a0e7-109">Access all your files in OneDrive without using local storage space.</span></span>
  