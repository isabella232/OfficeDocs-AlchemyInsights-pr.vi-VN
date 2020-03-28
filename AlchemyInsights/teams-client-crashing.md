---
title: Đội khách hàng bị rơi?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030758"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="56c3b-102">Đội khách hàng bị rơi?</span><span class="sxs-lookup"><span data-stu-id="56c3b-102">Teams client crashing?</span></span>

<span data-ttu-id="56c3b-103">Nếu khách hàng teams của bạn bị sập, hãy thử các cách sau:</span><span class="sxs-lookup"><span data-stu-id="56c3b-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="56c3b-104">Nếu bạn đang sử dụng ứng dụng teams trên máy tính để bàn, hãy đảm [bảo rằng ứng dụng được Cập Nhật hoàn toàn](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="56c3b-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="56c3b-105">Đảm bảo rằng tất cả các [văn phòng 365 URL và địa chỉ phạm vi](https://docs.microsoft.com/microsoftteams/connectivity-issues) có thể truy cập.</span><span class="sxs-lookup"><span data-stu-id="56c3b-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="56c3b-106">Đăng nhập bằng tài khoản quản trị của bạn và kiểm tra [bảng điều khiển dịch vụ y tế](https://docs.microsoft.com/office365/enterprise/view-service-health) để xác minh rằng không có sự cố hỏng hóc hoặc dịch vụ tồn tại.</span><span class="sxs-lookup"><span data-stu-id="56c3b-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="56c3b-107">Bước cuối cùng, bạn có thể cố gắng xóa bộ nhớ cache của máy khách teams:</span><span class="sxs-lookup"><span data-stu-id="56c3b-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="56c3b-108">Hoàn toàn thoát khỏi máy tính khách hàng Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="56c3b-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="56c3b-109">Bạn có thể bấm chuột phải vào **đội** từ khay biểu tượng và bấm **thoát**, hoặc chạy trình quản lý tác vụ và hoàn toàn giết quá trình.</span><span class="sxs-lookup"><span data-stu-id="56c3b-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="56c3b-110">Đi tới File Explorer, và gõ%appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="56c3b-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="56c3b-111">Một khi trong thư mục, bạn sẽ thấy một vài trong số các thư mục sau:</span><span class="sxs-lookup"><span data-stu-id="56c3b-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="56c3b-112">Từ trong **ứng dụng bộ nhớ cache**, đi đến bộ nhớ cache và xóa bất kỳ các tập tin trong vị trí bộ nhớ cache:%appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="56c3b-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="56c3b-113">Từ bên trong **Blob_storage**, xóa tất cả các tệp:%appdata%\Microsoft\teams\ blob_storage.</span><span class="sxs-lookup"><span data-stu-id="56c3b-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="56c3b-114">Từ trong **bộ nhớ cache**, xóa tất cả các tệp:%appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="56c3b-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="56c3b-115">Từ trong **cơ sở dữ liệu**, xóa tất cả các tệp:%appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="56c3b-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="56c3b-116">Từ bên trong **gpucache**, xóa tất cả các tệp:%appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="56c3b-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="56c3b-117">Từ trong **Indexeddb**, xoá tệp. db:%appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="56c3b-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="56c3b-118">Từ bên trong **lưu trữ cục bộ**, xóa tất cả các tệp:%appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="56c3b-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="56c3b-119">Cuối cùng, từ trong **tmp**, xóa bất kỳ tập tin:%appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="56c3b-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="56c3b-120">Khởi động lại máy khách teams của bạn.</span><span class="sxs-lookup"><span data-stu-id="56c3b-120">Restart your Teams client.</span></span>
