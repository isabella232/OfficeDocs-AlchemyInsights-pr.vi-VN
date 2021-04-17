---
title: Chứng chỉ liên kết ADFS được sắp hết hạn
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
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821973"
---
# <a name="adfs-federation-certificate-expiring"></a>Chứng chỉ liên kết ADFS được sắp hết hạn

Để giải quyết vấn đề này, hãy làm theo các bước sau đây:
  
1. Cài đặt mô-đun Microsoft Azure Active Directory cho Windows PowerShell trên máy tính (nếu mô-đun chưa được cài đặt). Để thực hiện thao tác này, hãy đi đến [quản lý AZURE AD bằng Windows PowerShell](https://aka.ms/aadposh).

2. Làm theo các bước trong "kịch bản 1: chứng chỉ ký mã hóa AD FS đã hết hạn" phần "của [" đã xảy ra sự cố khi truy nhập vào lỗi "site" từ AD FS khi một người dùng được liên kết đăng nhập vào Microsoft 365, Azure hoặc InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Làm theo các bước trong [Cập Nhật hoặc sửa chữa các thiết đặt của tên miền được liên kết trong Microsoft, Azure hoặc InTune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Để tìm hiểu thêm về việc gia hạn chứng chỉ liên kết, hãy xem gia [hạn chứng chỉ liên kết cho Microsoft 365 và Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
