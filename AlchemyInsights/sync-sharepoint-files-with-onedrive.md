---
title: Tập tin SharePoint Sync với khách hàng mới đồng bộ OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 74b79efeb7e46d03dc55f46252d152cd13e66c84
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757841"
---
# <a name="sync-sharepoint-files-with-the-new-onedrive-sync-client"></a><span data-ttu-id="5e1ad-102">Tập tin SharePoint Sync với khách hàng mới đồng bộ OneDrive</span><span class="sxs-lookup"><span data-stu-id="5e1ad-102">Sync SharePoint files with the new OneDrive sync client</span></span>

<span data-ttu-id="5e1ad-103">Mở với lệnh Explorer sẽ mở một trường hợp địa phương của Windows Explorer Hiển thị cấu trúc thư mục trên máy chủ máy chủ mà các trang web SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5e1ad-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="5e1ad-104">Điều này đang được nói, chúng tôi khuyên bạn [đồng bộ hóa tập tin SharePoint với khách hàng mới đồng bộ OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) </a> cung cấp [Các tập tin theo yêu cầu](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) bởi vì nó cung cấp địa phương truy cập tập tin của bạn và cung cấp hiệu suất tốt nhất.</span><span class="sxs-lookup"><span data-stu-id="5e1ad-104">This being said , we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="5e1ad-105">Nếu bạn đã chọn để sử dụng xem explorer thay vì sử dụng các khách hàng mới đồng bộ, đảm bảo bạn làm theo các bước và các thực tiễn tốt nhất trong các bài viết dưới đây.</span><span class="sxs-lookup"><span data-stu-id="5e1ad-105">If you chose to use explorer view instead of using the new sync client, ensure you follow the steps and best practices in the articles below.</span></span>

- [<span data-ttu-id="5e1ad-106">Làm thế nào để sử dụng lệnh "Mở với Explorer" để khắc phục sự cố trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5e1ad-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="5e1ad-107">Sao chép hoặc di chuyển các tập tin thư viện bằng cách sử dụng mở Explorer</span><span class="sxs-lookup"><span data-stu-id="5e1ad-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

<span data-ttu-id="5e1ad-108">Lưu ý: Mở Explorer nút không xuất hiện trong kinh nghiệm mới của thư viện.</span><span class="sxs-lookup"><span data-stu-id="5e1ad-108">Note:  The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="5e1ad-109">Bấm xem thả xuống ở phía trên bên phải (tên thay đổi thả xuống tùy thuộc vào dạng xem hiện thời của bạn), và sau đó bấm xem trong File Explorer.</span><span class="sxs-lookup"><span data-stu-id="5e1ad-109">Click the View drop-down in the upper right (the name of the drop-down changes depending on your current view), and then click View in File Explorer.</span></span>

 <span data-ttu-id="5e1ad-110">SharePoint mở Explorer sử dụng điều khiển ActiveX, do đó, nó chỉ được hỗ trợ trong Internet Explorer 10 hay 11.</span><span class="sxs-lookup"><span data-stu-id="5e1ad-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="5e1ad-111">Open Explorer không hoạt động trong Windows với Microsoft Edge, Google Chrome, Mozilla Firefox, hoặc trên các nền tảng Mac.</span><span class="sxs-lookup"><span data-stu-id="5e1ad-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="5e1ad-112">Vì lý do này, thám hiểm xem tùy chọn có thể được chuyển sang màu xám.</span><span class="sxs-lookup"><span data-stu-id="5e1ad-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

- <span data-ttu-id="5e1ad-113">[Tại sao SharePoint ribbon nút có sẵn hoặc chuyển sang màu xám](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="5e1ad-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

