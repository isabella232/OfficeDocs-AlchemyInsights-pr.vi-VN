---
title: Khắc phục sự cố "Mở với Explorer" các vấn đề trong SharePoint Online
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 52429314d1529d0d2df7886feaebbcfd27666a06
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559719"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="a9e07-102">Khắc phục sự cố "Mở với Explorer" các vấn đề trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a9e07-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="a9e07-103">Mở với lệnh Explorer sẽ mở một trường hợp địa phương của Windows Explorer Hiển thị cấu trúc thư mục trên máy chủ máy chủ mà các trang web SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a9e07-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="a9e07-104">Điều này đang được nói, chúng tôi khuyên bạn [đồng bộ hóa tập tin SharePoint với khách hàng mới đồng bộ OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) </a> cung cấp [Các tập tin theo yêu cầu](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) bởi vì nó cung cấp địa phương truy cập tập tin của bạn và cung cấp hiệu suất tốt nhất.</span><span class="sxs-lookup"><span data-stu-id="a9e07-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="a9e07-105">Nếu bạn đã chọn để sử dụng xem Explorer thay vì sử dụng khách hàng mới đồng bộ OneDrive, hãy chắc chắn rằng bạn làm theo các bước và các thực tiễn tốt nhất trong các bài viết sau đây:</span><span class="sxs-lookup"><span data-stu-id="a9e07-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="a9e07-106">Làm thế nào để sử dụng lệnh "Mở với Explorer" để khắc phục sự cố trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a9e07-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="a9e07-107">Sao chép hoặc di chuyển các tập tin thư viện bằng cách sử dụng mở Explorer</span><span class="sxs-lookup"><span data-stu-id="a9e07-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="a9e07-108">Nút **mở Explorer** không xuất hiện trong kinh nghiệm mới của thư viện.</span><span class="sxs-lookup"><span data-stu-id="a9e07-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="a9e07-109">Chọn chế độ **xem** thả xuống ở phía trên bên phải (tên thay đổi thả xuống tùy thuộc vào dạng xem hiện thời của bạn), và sau đó chọn **chế độ xem trong File Explorer**.</span><span class="sxs-lookup"><span data-stu-id="a9e07-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="a9e07-110">SharePoint mở Explorer sử dụng điều khiển ActiveX, do đó, nó chỉ được hỗ trợ trong Internet Explorer 10 hay 11.</span><span class="sxs-lookup"><span data-stu-id="a9e07-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="a9e07-111">Open Explorer không hoạt động trong Windows với Microsoft Edge, Google Chrome, Mozilla Firefox, hoặc trên các nền tảng Mac.</span><span class="sxs-lookup"><span data-stu-id="a9e07-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="a9e07-112">Vì lý do này, thám hiểm xem tùy chọn có thể được chuyển sang màu xám.</span><span class="sxs-lookup"><span data-stu-id="a9e07-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="a9e07-113">[Tại sao SharePoint ribbon nút có sẵn hoặc chuyển sang màu xám](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="a9e07-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

