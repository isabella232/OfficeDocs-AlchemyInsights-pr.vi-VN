---
title: ADFS liên chứng chỉ hết hạn
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 55529265d2356a911624026107fb639f93e29abd
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925402"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS liên chứng chỉ hết hạn

Để giải quyết vấn đề này, hãy làm theo các bước sau:
  
1. Cài đặt các Microsoft Azure Active Directory Module cho Windows PowerShell trên máy tính (nếu các mô-đun đã không được cài đặt). Để làm điều này, hãy [quản lý Azure quảng cáo bằng cách sử dụng Windows PowerShell](https://aka.ms/aadposh).
    
2. Làm theo các bước trong những "kịch bản 1: AD FS token-ký chứng chỉ hết hạn" phần ["Đã có một vấn đề khi truy cập các trang web"](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)lỗi từ AD FS khi người dùng đã liên kết đăng nhập Office 365, Azure, hoặc dành.
    
3. Làm theo các bước làm thế nào [để cập nhật hoặc sửa chữa cài đặt của một tên miền đã liên kết trong Office 365, Azure, hoặc dành](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
    Để tìm hiểu thêm về đổi mới liên chứng chỉ, hãy xem [Renew liên chứng chỉ cho Office 365 và Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
    

