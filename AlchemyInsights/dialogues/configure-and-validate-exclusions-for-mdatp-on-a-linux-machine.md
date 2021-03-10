---
title: Cấu hình và xác thực loại trừ cho MDATP trên máy Linux
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696075"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a>Cấu hình và xác thực loại trừ cho MDATP trên máy Linux

Bạn có thể loại trừ các tệp nhất định, thư mục, quy trình và các tệp mở quá trình từ quét MDATP. Việc loại trừ giúp tránh phát hiện không chính xác các phần mềm và tệp riêng biệt hoặc tùy chỉnh cho tổ chức của bạn. Việc loại trừ cũng giúp giảm thiểu các vấn đề về hiệu suất do MDATP gây ra.

Để tìm hiểu thêm, hãy xem [cấu hình và xác thực các loại trừ cho MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).

> [!IMPORTANT]
> Các loại trừ được mô tả trong bài viết này không áp dụng cho các chức năng khác của MDATP for Linux, bao gồm Endpoint Detection and Response (EDR). Các tệp mà bạn loại trừ bằng cách sử dụng các phương pháp được mô tả trong bài viết này vẫn có thể kích hoạt cảnh báo EDR và các chức năng phát hiện khác.
