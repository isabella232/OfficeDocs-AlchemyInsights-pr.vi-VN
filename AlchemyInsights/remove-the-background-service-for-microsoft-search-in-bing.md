---
title: Loại bỏ dịch vụ nền cho tìm kiếm Microsoft trong Bing
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
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816343"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Loại bỏ dịch vụ nền cho tìm kiếm Microsoft trong Bing

Để loại bỏ dịch vụ nền cho Microsoft Search trong Bing, bạn có thể thử các biện pháp sau đây:

1. Để trở về thiết đặt công cụ tìm kiếm ban đầu, hãy thực hiện các thao tác sau:

    một. Chuyển đổi **sử dụng Bing làm công cụ tìm [kiếm](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) mặc định của bạn tắt**.

    b. [Đi đến Trung tâm quản trị Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) và xóa các thiết đặt ảnh hưởng đến tất cả người dùng trong tổ chức của bạn.

2. Để loại bỏ dịch vụ nền khỏi thiết bị riêng lẻ, hãy thực hiện các tác vụ sau đây:

    một. Chọn **Pa-nen điều khiển > chương trình > các chương trình và tính năng**.

    b. Bấm chuột phải vào **Microsoft Search trong Bing** bên dưới danh sách các chương trình đã cài đặt, rồi bấm vào **gỡ cài đặt**.

3. Để loại bỏ dịch vụ nền khỏi nhiều thiết bị trong tổ chức của bạn, hãy đăng nhập với tư cách là người quản trị và chạy lệnh sau đây trong một tập lệnh: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
