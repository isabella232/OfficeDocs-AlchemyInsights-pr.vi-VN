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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/15/2019
ms.locfileid: "36737211"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="0acbf-102">Chứng chỉ liên kết ADFS hết hạn</span><span class="sxs-lookup"><span data-stu-id="0acbf-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="0acbf-103">Để khắc phục sự cố này, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="0acbf-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="0acbf-104">Cài đặt Microsoft Azure Active Directory mô-đun Windows PowerShell trên máy tính (nếu mô-đun chưa được cài đặt).</span><span class="sxs-lookup"><span data-stu-id="0acbf-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="0acbf-105">Để thực hiện việc này, hãy đi tới [quản lý AZURE AD bằng Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="0acbf-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="0acbf-106">Làm theo các bước trong phần "tình huống 1: AD FS mã thông báo ký chứng chỉ hết hạn" của ["đã có sự cố truy cập vào trang web" lỗi từ AD FS khi người dùng liên kết đăng nhập vào Office 365, Azure hoặc InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="0acbf-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="0acbf-107">Làm theo các bước trong [bản Cập Nhật hoặc sửa chữa cài đặt của một liên kết miền trong Office 365, Azure hoặc InTune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="0acbf-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="0acbf-108">Để tìm hiểu thêm về tái tạo chứng chỉ liên kết, hãy xem gia [hạn chứng chỉ liên kết cho Office 365 và Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="0acbf-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
