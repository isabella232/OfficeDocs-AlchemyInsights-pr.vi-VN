---
title: Sửa đổi Microsoft Edge dùng biến thư mục dữ liệu thay vì đường dẫn mã cứng
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 235696d17711726da57d9a09c23b5b13140a28d7645299ef120a4b2c7b395c5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54113438"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Sửa đổi Microsoft Edge dùng biến thư mục dữ liệu thay vì đường dẫn mã cứng

Ví dụ: trên Windows, để lưu trữ dữ liệu hồ sơ dưới dữ liệu ứng dụng cục bộ của người dùng thay vì tại vị trí mặc định, hãy đặt chính sách **UserDataDir** **thành ${local_app_data}\Edge\Profile**. 

Để tìm hiểu thêm, hãy [xem mục Tạo Microsoft Edge thư mục dữ liệu người dùng .](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars)