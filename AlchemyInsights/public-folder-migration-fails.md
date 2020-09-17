---
title: Di chuyển thư mục công cộng không thành công tại 95%
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: b22dce778b4507e0a3337a59a55531ce248b59c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47803929"
---
# <a name="public-folder-migration-fails-at-95"></a>Di chuyển thư mục công cộng không thành công tại 95%

Bạn có thể đã bắt đầu hoàn thành một lô di chuyển và trạng thái của lô di chuyển vẫn tiếp **tục hiển thị** được đồng bộ trong một thời gian rất dài. Đây là hành vi dự kiến.

Nó phổ **biến cho trạng** Thái của lô di chuyển vẫn tiếp tục được đồng bộ trong một vài giờ trước khi chuyển đổi để **hoàn thành**. Để di chuyển liên quan đến một số lượng lớn các hộp thư đích, thông thường là bạn sẽ thấy trạng thái vẫn giữ nguyên trong trạng thái đồng bộ trong hơn 24 giờ, không cung cấp các yêu cầu di chuyển thư mục công cộng nằm bên dưới. Vui lòng cho phép 24-48 giờ cho lô di chuyển để hoàn thành nhiệm vụ.

Đối với việc di chuyển thư mục công cộng không tại 95%, với lỗi FailedToMailEnablePublicFoldersException:

1. Tải xuống và chạy tập lệnh [thư mục Validatemailenabledtại](https://aka.ms/ValidateMEPF) máy chủ Exchange tại cơ sở của bạn.

2. Thực hiện các hành động khắc phục được đề xuất bởi tập lệnh.

3. Chạy thư mục đồng bộ (dành cho Exchange 2010) hoặc thư mục đồng bộ hóa (dành cho Exchange 2013 trở lên).

4. Tiếp tục di chuyển thư mục công cộng.
