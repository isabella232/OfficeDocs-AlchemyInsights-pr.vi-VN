---
title: Khắc phục sự cố "mở với Explorer" các vấn đề trong SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: ba9f11da5c35c3681e9bd5ceaf13233fe8b80fc9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737327"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="a6d79-102">Khắc phục sự cố "mở với Explorer" các vấn đề trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a6d79-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="a6d79-103">Chúng tôi khuyên bạn nên [đồng bộ các tệp SharePoint với máy khách đồng bộ OneDrive mới](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) cung cấp các [tệp theo yêu cầu](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) vì nó cung cấp quyền truy nhập cục bộ vào tệp của bạn và cung cấp hiệu suất tốt nhất.</span><span class="sxs-lookup"><span data-stu-id="a6d79-103">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>

<span data-ttu-id="a6d79-104">Để khắc phục sự cố khi mở với vấn đề về Explorer, hãy làm theo các bước và thực hành tốt nhất trong các bài viết sau đây:</span><span class="sxs-lookup"><span data-stu-id="a6d79-104">To troubleshoot Open with Explorer issues, follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="a6d79-105">Cách dùng lệnh "mở bằng Explorer" để khắc phục sự cố trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a6d79-105">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)
- [<span data-ttu-id="a6d79-106">Sao chép hoặc di chuyển tệp thư viện bằng cách sử dụng mở bằng Explorer</span><span class="sxs-lookup"><span data-stu-id="a6d79-106">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> <span data-ttu-id="a6d79-107">**Yù**</span><span class="sxs-lookup"><span data-stu-id="a6d79-107">**Note:**</span></span>
>- <span data-ttu-id="a6d79-108">Mở với Explorer chỉ được hỗ trợ trong Internet Explorer 10 hoặc 11.</span><span class="sxs-lookup"><span data-stu-id="a6d79-108">Open with Explorer is only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="a6d79-109">Mở với Explorer không hoạt động trong Windows với Microsoft Edge, Google Chrome, Mozilla Firefox hoặc trên nền tảng Mac.</span><span class="sxs-lookup"><span data-stu-id="a6d79-109">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="a6d79-110">Vì lý do này, tùy chọn dạng xem Explorer có thể bị mờ đi.</span><span class="sxs-lookup"><span data-stu-id="a6d79-110">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
>- <span data-ttu-id="a6d79-111">Nút mở với Explorer không xuất hiện trong trải nghiệm thư viện mới.</span><span class="sxs-lookup"><span data-stu-id="a6d79-111">The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="a6d79-112">Chọn danh sách thả xuống **dạng xem** ở phía trên bên phải (tên của các thay đổi thả xuống tùy thuộc vào dạng xem hiện tại của bạn), rồi chọn **xem trong file Explorer**.</span><span class="sxs-lookup"><span data-stu-id="a6d79-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
