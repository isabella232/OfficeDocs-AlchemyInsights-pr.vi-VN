---
title: Chứng chỉ liên kết ADFS hết hạn
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737211"
---
# <a name="adfs-federation-certificate-expiring"></a>Chứng chỉ liên kết ADFS hết hạn

Để khắc phục sự cố này, hãy làm theo các bước sau:
  
1. Cài đặt Microsoft Azure Active Directory mô-đun Windows PowerShell trên máy tính (nếu mô-đun chưa được cài đặt). Để thực hiện việc này, hãy đi tới [quản lý AZURE AD bằng Windows PowerShell](https://aka.ms/aadposh).

2. Làm theo các bước trong phần "tình huống 1: AD FS mã thông báo ký chứng chỉ hết hạn" của ["đã có sự cố truy cập vào trang web" lỗi từ AD FS khi người dùng liên kết đăng nhập vào Office 365, Azure hoặc InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Làm theo các bước trong [bản Cập Nhật hoặc sửa chữa cài đặt của một liên kết miền trong Office 365, Azure hoặc InTune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Để tìm hiểu thêm về tái tạo chứng chỉ liên kết, hãy xem gia [hạn chứng chỉ liên kết cho Office 365 và Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
