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
ms.custom:
- "6462"
- "9003546"
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: ea93bb6f3cbbc3424f5e006ffac482a7445c8164
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086070"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="2ca75-102">Khắc phục sự cố "mở với Explorer" các vấn đề trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2ca75-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="2ca75-103">Làm theo các bước và cách thực hành tốt nhất trong các bài viết sau đây:</span><span class="sxs-lookup"><span data-stu-id="2ca75-103">Follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="2ca75-104">Cách dùng lệnh "mở bằng Explorer" để khắc phục sự cố trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2ca75-104">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)

- [<span data-ttu-id="2ca75-105">Sao chép hoặc di chuyển tệp thư viện bằng cách sử dụng mở bằng Explorer</span><span class="sxs-lookup"><span data-stu-id="2ca75-105">Copy or move library files by using Open with Explorer</span></span>](https://support.microsoft.com/office/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2?ui=en-us&rs=en-us&ad=us)

> [!NOTE]
- <span data-ttu-id="2ca75-106">Chúng tôi khuyên bạn nên đồng bộ các [tệp SharePoint với máy khách đồng bộ OneDrive mới](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us) cung cấp các [tệp theo yêu cầu](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us) vì việc đồng bộ hóa quyền truy nhập cục bộ vào các tệp của bạn và cung cấp hiệu suất tốt nhất.</span><span class="sxs-lookup"><span data-stu-id="2ca75-106">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us) which provides [Files On-Demand](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us) because the synchronization grants local access to your files and offers the best performance.</span></span>

- <span data-ttu-id="2ca75-107">**Mở với Explorer** chỉ được hỗ trợ trong Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="2ca75-107">**Open with Explorer** is only supported in Internet Explorer 11.</span></span> <span data-ttu-id="2ca75-108">Để biết thêm thông tin, hãy xem [phần kết thúc hỗ trợ cho IE11 với các ứng dụng Microsoft 365](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy)).</span><span class="sxs-lookup"><span data-stu-id="2ca75-108">For more information, see [end of support for IE11 with Microsoft 365 Apps](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy)).</span></span> <span data-ttu-id="2ca75-109">**Mở với Explorer** không hoạt động trong Windows với Microsoft Edge, Google Chrome, Mozilla Firefox hoặc trên nền tảng Mac.</span><span class="sxs-lookup"><span data-stu-id="2ca75-109">**Open with Explorer** doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="2ca75-110">Vì lý do này, tùy chọn **dạng xem Explorer** có thể bị mờ đi.</span><span class="sxs-lookup"><span data-stu-id="2ca75-110">Due to this reason, the **Explorer View** option may be grayed out.</span></span> 

- <span data-ttu-id="2ca75-111">Nút **mở với Explorer** không xuất hiện trong trải nghiệm thư viện mới.</span><span class="sxs-lookup"><span data-stu-id="2ca75-111">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="2ca75-112">Chọn danh sách thả xuống **dạng xem** ở phía trên bên phải (tên của các thay đổi thả xuống tùy thuộc vào dạng xem hiện tại của bạn), rồi chọn **xem trong file Explorer**.</span><span class="sxs-lookup"><span data-stu-id="2ca75-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>

