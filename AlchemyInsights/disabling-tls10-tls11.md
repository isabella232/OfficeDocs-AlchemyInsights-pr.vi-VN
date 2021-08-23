---
title: Tắt TLS1.0 và TLS 1.1 cho việc gửi máy khách SMTP AUTH
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13649"
- "9005383"
ms.openlocfilehash: 6751f4e8a177958fdec674899606252a4ae40a72
ms.sourcegitcommit: d9e6f700cd73a61c109e2a99bc71e559dba34722
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/18/2021
ms.locfileid: "58455130"
---
# <a name="disabling-tls10-and-tls-11-for-smtp-auth-client-submission"></a>Tắt TLS1.0 và TLS 1.1 cho việc gửi máy khách SMTP AUTH

Gần đây, chúng tôi đã bắt đầu vô hiệu hóa TLS1.0 và TLS 1.1 cho việc gửi máy khách SMTP AUTH. 

Nếu bạn đã cấu hình một thiết bị, ứng dụng hoặc máy chủ gửi email tới Microsoft 365 bằng cách sử dụng phương pháp gửi máy khách SMTP AUTH, hãy đảm bảo thiết bị, ứng dụng hoặc máy chủ của bạn hỗ trợ TLS 1.2 cho SMTP. 