---
title: Loại bỏ dịch vụ nền để Tìm kiếm của Microsoft trong Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 07d24290fc3b13cce7a931c4cff15176c080b4413489ba1935b6886939ea3874
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53982395"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Loại bỏ dịch vụ nền để Tìm kiếm của Microsoft trong Bing

Để loại bỏ dịch vụ nền cho Tìm kiếm của Microsoft trong Bing, bạn có thể thử các biện pháp khắc phục sau đây:

1. Để hoàn nguyên về cài đặt công cụ tìm kiếm ban đầu, hãy thực hiện các bước sau:

    a. Chuyển nút bật **tắt Sử Bing làm công cụ tìm kiếm mặc định của [bạn.](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**

    b. [Đi tới trang Trung tâm quản trị Microsoft 365 rồi](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) xóa cài đặt ảnh hưởng đến tất cả người dùng trong tổ chức của bạn.

2. Để loại bỏ dịch vụ nền khỏi một thiết bị riêng lẻ, hãy thực hiện các tác vụ sau đây:

    a. Chọn **Panel Điều khiển > Trình và > Chương trình và Tính năng**.

    b. Bấm chuột phải vào **Tìm kiếm của Microsoft xem Bing** danh sách các chương trình đã cài đặt, rồi bấm Dỡ cài **đặt.**

3. Để loại bỏ dịch vụ nền khỏi nhiều thiết bị trong tổ chức của bạn, hãy đăng nhập với tư cách người quản trị và chạy lệnh sau đây trong một tập lệnh: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
