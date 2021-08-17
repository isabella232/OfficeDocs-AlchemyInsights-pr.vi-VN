---
title: Tập hợp bản sao
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110702"
---
# <a name="replica-set"></a>Tập hợp bản sao

AADDS còn được gọi là tên miền được quản lý. Thực tế là hai bộ điều khiển miền được chạy và duy trì bởi bộ điều khiển phụ trợ. Hai DC bao gồm một DC chính và một DC bản sao. Các bản sao lưu trong AADDS (tên miền được quản lý) là một quy trình tự động do nền tảng Azure quản lý. Trong trường hợp có sự cố với miền được quản lý của bạn, bộ máy hỗ trợ của Azure có thể hỗ trợ bạn trong việc khôi phục từ bản sao lưu.

Bạn tạo mỗi bản sao trong một mạng ảo. Mỗi mạng ảo phải được ngang hàng với mọi mạng ảo khác lưu trữ bộ bản sao của tên miền được quản lý. Cấu hình này tạo ra cấu hình mạng lưới hỗ trợ nhân bản thư mục. Một mạng ảo có thể hỗ trợ nhiều bộ bản sao, miễn là mỗi bộ bản sao nằm trong một mạng con ảo khác nhau.

Để biết thêm chi tiết về bộ Bản sao, hãy [xem Bản sao khái niệm .](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
