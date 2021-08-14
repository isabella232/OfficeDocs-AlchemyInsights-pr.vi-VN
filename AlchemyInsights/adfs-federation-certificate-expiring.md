---
title: Chứng chỉ Liên kết ADFS hết hạn
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952991"
---
# <a name="adfs-federation-certificate-expiring"></a>Chứng chỉ Liên kết ADFS hết hạn

Để giải quyết vấn đề này, hãy làm theo các bước sau:
  
1. Cài đặt Mô-Microsoft Azure Active Directory cho Windows PowerShell trên máy tính (nếu mô-đun chưa được cài đặt). Để thực hiện điều này, hãy đi [tới Quản lý Azure AD bằng Windows PowerShell.](https://aka.ms/aadposh)

2. Làm theo các bước trong mục "Kịch bản 1: Chứng chỉ ký mã thông báo AD FS đã hết hạn" của lỗi "Đã xảy ra sự cố khi truy nhập site" từ AD FS khi người dùng được liên kết đăng nhập vào [Microsoft 365, Azure hoặc Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Làm theo các bước trong Cập nhật hoặc sửa chữa cài đặt miền được liên kết trong [Microsoft, Azure hoặc Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Để tìm hiểu thêm về việc gia hạn chứng chỉ liên kết, hãy [xem mục Gia hạn chứng chỉ liên kết cho Microsoft 365 và Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
