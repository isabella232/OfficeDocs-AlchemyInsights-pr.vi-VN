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
# <a name="teams-client-crashing"></a>Đội khách hàng bị rơi?

Nếu khách hàng teams của bạn bị sập, hãy thử các cách sau:

- Nếu bạn đang sử dụng ứng dụng teams trên máy tính để bàn, hãy đảm [bảo rằng ứng dụng được Cập Nhật hoàn toàn](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Đảm bảo rằng tất cả các [văn phòng 365 URL và địa chỉ phạm vi](https://docs.microsoft.com/microsoftteams/connectivity-issues) có thể truy cập.

- Đăng nhập bằng tài khoản quản trị của bạn và kiểm tra [bảng điều khiển dịch vụ y tế](https://docs.microsoft.com/office365/enterprise/view-service-health) để xác minh rằng không có sự cố hỏng hóc hoặc dịch vụ tồn tại.

 - Bước cuối cùng, bạn có thể cố gắng xóa bộ nhớ cache của máy khách teams:

    1.  Hoàn toàn thoát khỏi máy tính khách hàng Microsoft teams. Bạn có thể bấm chuột phải vào **đội** từ khay biểu tượng và bấm **thoát**, hoặc chạy trình quản lý tác vụ và hoàn toàn giết quá trình.

    2.  Đi tới File Explorer, và gõ%appdata%\Microsoft\teams.

    3.  Một khi trong thư mục, bạn sẽ thấy một vài trong số các thư mục sau:

         - Từ trong **ứng dụng bộ nhớ cache**, đi đến bộ nhớ cache và xóa bất kỳ các tập tin trong vị trí bộ nhớ cache:%appdata%\Microsoft\teams\application cache\cache.

        - Từ bên trong **Blob_storage**, xóa tất cả các tệp:%appdata%\Microsoft\teams\ blob_storage.

        - Từ trong **bộ nhớ cache**, xóa tất cả các tệp:%appdata%\Microsoft\teams\Cache.

        - Từ trong **cơ sở dữ liệu**, xóa tất cả các tệp:%appdata%\Microsoft\teams\databases.

        - Từ bên trong **gpucache**, xóa tất cả các tệp:%appdata%\Microsoft\teams\GPUcache.

        - Từ trong **Indexeddb**, xoá tệp. db:%appdata%\Microsoft\teams\IndexedDB.

        - Từ bên trong **lưu trữ cục bộ**, xóa tất cả các tệp:%appdata%\Microsoft\teams\Local Storage.

        - Cuối cùng, từ trong **tmp**, xóa bất kỳ tập tin:%appdata%\Microsoft\teams\tmp.

    4. Khởi động lại máy khách teams của bạn.
