---
title: Chứng chỉ liên kết ADFS được sắp hết hạn
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686805"
---
# <a name="adfs-federation-certificate-expiring"></a>Chứng chỉ liên kết ADFS được sắp hết hạn

Để giải quyết vấn đề này, hãy làm theo các bước sau đây:
  
1. Cài đặt mô-đun Microsoft Azure Active Directory cho Windows PowerShell trên máy tính (nếu mô-đun chưa được cài đặt). Để thực hiện thao tác này, hãy đi đến [quản lý AZURE AD bằng Windows PowerShell](https://aka.ms/aadposh).

2. Làm theo các bước trong "kịch bản 1: chứng chỉ ký mã hóa AD FS đã hết hạn" phần "của [" đã xảy ra sự cố khi truy nhập vào lỗi "site" từ AD FS khi một người dùng được liên kết đăng nhập vào Microsoft 365, Azure hoặc InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Làm theo các bước trong [Cập Nhật hoặc sửa chữa các thiết đặt của tên miền được liên kết trong Microsoft, Azure hoặc InTune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Để tìm hiểu thêm về việc gia hạn chứng chỉ liên kết, hãy xem gia [hạn chứng chỉ liên kết cho Microsoft 365 và Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
