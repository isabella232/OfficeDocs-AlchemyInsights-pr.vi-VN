---
title: Khắc phục sự cố "mở với Explorer" trong SharePoint trực tuyến
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 08/07/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 09d0d76f8c61f7fcd21a58527e220b65f123654d
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770301"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="d79f0-102">Khắc phục sự cố "mở với Explorer" trong SharePoint trực tuyến</span><span class="sxs-lookup"><span data-stu-id="d79f0-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="d79f0-103">Chúng tôi khuyên bạn nên [đồng bộ hoá tệp SharePoint với khách hàng Sync mới OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) cung cấp [tệp theo yêu cầu](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) vì nó cung cấp truy cập Cục bộ vào tệp của bạn và cung cấp hiệu suất tốt nhất.</span><span class="sxs-lookup"><span data-stu-id="d79f0-103">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>

<span data-ttu-id="d79f0-104">Để khắc phục sự cố mở với Explorer, hãy làm theo các bước và thực tiễn tốt nhất trong bài viết sau đây:</span><span class="sxs-lookup"><span data-stu-id="d79f0-104">To troubleshoot Open with Explorer issues, follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="d79f0-105">Làm thế nào để sử dụng lệnh "mở với Explorer" để khắc phục sự cố trong SharePoint trực tuyến</span><span class="sxs-lookup"><span data-stu-id="d79f0-105">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)
- [<span data-ttu-id="d79f0-106">Sao chép hoặc di chuyển tệp thư viện bằng cách sử dụng mở với Explorer</span><span class="sxs-lookup"><span data-stu-id="d79f0-106">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> <span data-ttu-id="d79f0-107">**Lưu ý:**</span><span class="sxs-lookup"><span data-stu-id="d79f0-107">**Note:**</span></span>
>
>- <span data-ttu-id="d79f0-108">Nút mở Explorer không xuất hiện trong trải nghiệm thư viện mới.</span><span class="sxs-lookup"><span data-stu-id="d79f0-108">The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="d79f0-109">Chọn menu thả xuống dạng **xem** ở phía trên bên phải (tên của các thay đổi thả xuống tùy thuộc vào dạng xem hiện tại của bạn), sau đó chọn **xem trong file Explorer**.</span><span class="sxs-lookup"><span data-stu-id="d79f0-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
>- <span data-ttu-id="d79f0-110">Mở bằng Explorer chỉ được hỗ trợ trong Internet Explorer 10 hoặc 11.</span><span class="sxs-lookup"><span data-stu-id="d79f0-110">Open with Explorer is only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="d79f0-111">Mở bằng Explorer không hoạt động trong Windows với Microsoft Edge, Google Chrome, Mozilla Firefox hoặc trên nền tảng Mac.</span><span class="sxs-lookup"><span data-stu-id="d79f0-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="d79f0-112">Vì lý do này, tùy chọn Explorer View có thể được chuyển sang màu xám.</span><span class="sxs-lookup"><span data-stu-id="d79f0-112">Due to this reason, the Explorer View option may be grayed out.</span></span>


