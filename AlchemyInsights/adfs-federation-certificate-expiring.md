---
title: ADFS liên chứng chỉ hết hạn
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c608489be8497233d9d4f87ec53649026b823250
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29497174"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="9cfba-102">ADFS liên chứng chỉ hết hạn</span><span class="sxs-lookup"><span data-stu-id="9cfba-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="9cfba-103">Để giải quyết vấn đề này, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="9cfba-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="9cfba-p101">Cài đặt các Microsoft Azure Active Directory Module cho Windows PowerShell trên máy tính (nếu các mô-đun đã không được cài đặt). Để làm điều này, hãy [quản lý Azure quảng cáo bằng cách sử dụng Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="9cfba-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>
    
2. <span data-ttu-id="9cfba-106">Làm theo các bước trong những "kịch bản 1: AD FS token-ký chứng chỉ hết hạn" phần ["Đã có một vấn đề khi truy cập các trang web"](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)lỗi từ AD FS khi người dùng đã liên kết đăng nhập Office 365, Azure, hoặc dành.</span><span class="sxs-lookup"><span data-stu-id="9cfba-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
3. <span data-ttu-id="9cfba-107">Làm theo các bước làm thế nào [để cập nhật hoặc sửa chữa cài đặt của một tên miền đã liên kết trong Office 365, Azure, hoặc dành](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="9cfba-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
    <span data-ttu-id="9cfba-108">Để tìm hiểu thêm về đổi mới liên chứng chỉ, hãy xem [Renew liên chứng chỉ cho Office 365 và Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="9cfba-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
    

