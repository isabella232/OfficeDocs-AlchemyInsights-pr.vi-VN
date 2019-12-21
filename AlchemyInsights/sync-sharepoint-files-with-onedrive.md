---
title: Khắc phục sự cố "mở với Explorer" trong SharePoint trực tuyến
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 21a0c193b752342d47189dda73d171249153f7fc
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/20/2019
ms.locfileid: "40050835"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="bf8a2-102">Khắc phục sự cố "mở với Explorer" trong SharePoint trực tuyến</span><span class="sxs-lookup"><span data-stu-id="bf8a2-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="bf8a2-103">Lệnh mở với Explorer mở một phiên bản địa phương của Windows Explorer Hiển thị cấu trúc thư mục trên máy chủ lưu trữ các trang web SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bf8a2-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="bf8a2-104">Điều này được cho biết, chúng tôi khuyên bạn nên</a> [đồng bộ hóa tệp SharePoint với khách hàng Sync mới OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) cung cấp [tệp theo yêu cầu](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) vì nó cung cấp quyền truy cập Cục bộ vào tệp của bạn và cung cấp hiệu suất tốt nhất.</span><span class="sxs-lookup"><span data-stu-id="bf8a2-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="bf8a2-105">Nếu bạn chọn sử dụng Explorer xem thay vì sử dụng máy khách đồng bộ OneDrive mới, đảm bảo rằng bạn làm theo các bước và thực tiễn tốt nhất trong bài viết sau đây:</span><span class="sxs-lookup"><span data-stu-id="bf8a2-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="bf8a2-106">Làm thế nào để sử dụng lệnh "mở với Explorer" để khắc phục sự cố trong SharePoint trực tuyến</span><span class="sxs-lookup"><span data-stu-id="bf8a2-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)

- [<span data-ttu-id="bf8a2-107">Sao chép hoặc di chuyển tệp thư viện bằng cách sử dụng mở với Explorer</span><span class="sxs-lookup"><span data-stu-id="bf8a2-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="bf8a2-108">Nút **mở với Explorer** không xuất hiện trong trải nghiệm thư viện mới.</span><span class="sxs-lookup"><span data-stu-id="bf8a2-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="bf8a2-109">Chọn menu thả xuống dạng **xem** ở phía trên bên phải (tên của các thay đổi thả xuống tùy thuộc vào dạng xem hiện tại của bạn), sau đó chọn **xem trong file Explorer**.</span><span class="sxs-lookup"><span data-stu-id="bf8a2-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="bf8a2-110">SharePoint mở với Explorer sử dụng điều khiển ActiveX, vì vậy nó chỉ được hỗ trợ trong Internet Explorer 10 hoặc 11.</span><span class="sxs-lookup"><span data-stu-id="bf8a2-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="bf8a2-111">Mở bằng Explorer không hoạt động trong Windows với Microsoft Edge, Google Chrome, Mozilla Firefox hoặc trên nền tảng Mac.</span><span class="sxs-lookup"><span data-stu-id="bf8a2-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="bf8a2-112">Vì lý do này, tùy chọn Explorer View có thể được chuyển sang màu xám.</span><span class="sxs-lookup"><span data-stu-id="bf8a2-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="bf8a2-113">[Tại sao SharePoint ruy băng nút có sẵn hoặc màu xám](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="bf8a2-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

