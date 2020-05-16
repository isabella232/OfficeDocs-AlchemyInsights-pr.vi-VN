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
ms.openlocfilehash: c49dfbf422b312f4744711d5f12b0eb83b6ebf2e
ms.sourcegitcommit: b398afd92d4259f893c25b48aec65921e6cc68d6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/16/2020
ms.locfileid: "44268794"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="f4b8e-102">Đội khách hàng bị rơi?</span><span class="sxs-lookup"><span data-stu-id="f4b8e-102">Teams client crashing?</span></span>

<span data-ttu-id="f4b8e-103">Nếu khách hàng teams của bạn bị sập, hãy thử các cách sau:</span><span class="sxs-lookup"><span data-stu-id="f4b8e-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="f4b8e-104">Nếu bạn đang sử dụng ứng dụng teams trên máy tính để bàn, hãy đảm [bảo rằng ứng dụng được Cập Nhật hoàn toàn](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="f4b8e-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="f4b8e-105">Đảm bảo rằng tất cả các [URL của Microsoft 365 và phạm vi địa chỉ](https://docs.microsoft.com/microsoftteams/connectivity-issues) có thể truy cập.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="f4b8e-106">Đăng nhập bằng tài khoản quản trị viên của bạn và kiểm tra [bảng điều khiển dịch vụ y tế](https://docs.microsoft.com/office365/enterprise/view-service-health) để xác minh rằng không có sự cố hỏng hóc hoặc dịch vụ tồn tại.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="f4b8e-107">Bước cuối cùng, bạn có thể cố gắng xóa bộ nhớ cache của máy khách teams:</span><span class="sxs-lookup"><span data-stu-id="f4b8e-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="f4b8e-108">Hoàn toàn thoát khỏi máy tính khách hàng Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="f4b8e-109">Bạn có thể bấm chuột phải vào **đội** từ khay biểu tượng và bấm **thoát**, hoặc chạy trình quản lý tác vụ và hoàn toàn giết quá trình.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="f4b8e-110">Đi tới File Explorer, và gõ%appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="f4b8e-111">Một khi trong thư mục, bạn sẽ thấy một vài trong số các thư mục sau:</span><span class="sxs-lookup"><span data-stu-id="f4b8e-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="f4b8e-112">Từ trong **ứng dụng bộ nhớ cache**, đi đến bộ nhớ cache và xóa bất kỳ các tập tin trong vị trí bộ nhớ cache:%appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="f4b8e-113">Từ bên trong **Blob_storage**, xóa tất cả các tệp:%appdata%\Microsoft\teams\ blob_storage.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="f4b8e-114">Từ trong **bộ nhớ cache**, xóa tất cả các tệp:%appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="f4b8e-115">Từ trong **cơ sở dữ liệu**, xóa tất cả các tệp:%appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="f4b8e-116">Từ bên trong **gpucache**, xóa tất cả các tệp:%appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="f4b8e-117">Từ trong **Indexeddb**, xoá tệp. db:%appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="f4b8e-118">Từ bên trong **lưu trữ cục bộ**, xóa tất cả các tệp:%appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="f4b8e-119">Cuối cùng, từ trong **tmp**, xóa bất kỳ tập tin:%appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="f4b8e-120">Khởi động lại máy khách teams của bạn.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-120">Restart your Teams client.</span></span>

<span data-ttu-id="f4b8e-121">Nếu khách hàng teams của bạn vẫn bị sập, bạn có thể tạo lại sự cố không?</span><span class="sxs-lookup"><span data-stu-id="f4b8e-121">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="f4b8e-122">Nếu có:</span><span class="sxs-lookup"><span data-stu-id="f4b8e-122">If so:</span></span> 

1. <span data-ttu-id="f4b8e-123">Sử dụng trình ghi bước để nắm bắt các bước của bạn.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-123">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="f4b8e-124">Đóng tất cả các ứng dụng không cần thiết hoặc bí mật.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-124">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="f4b8e-125">Khởi động trình ghi bước và tái tạo sự cố khi đăng nhập bằng tài khoản người dùng bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-125">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    
2. <span data-ttu-id="f4b8e-126">Đính kèm tập tin vào trường hợp hỗ trợ của bạn.</span><span class="sxs-lookup"><span data-stu-id="f4b8e-126">Attach the file to your support case.</span></span>
