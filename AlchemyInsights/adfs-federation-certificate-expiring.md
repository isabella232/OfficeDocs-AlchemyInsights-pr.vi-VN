---
title: Chứng chỉ liên kết ADFS hết hạn
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710429"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="93f65-102">Chứng chỉ liên kết ADFS hết hạn</span><span class="sxs-lookup"><span data-stu-id="93f65-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="93f65-103">Để khắc phục sự cố này, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="93f65-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="93f65-104">Cài đặt Microsoft Azure Active Directory mô-đun Windows PowerShell trên máy tính (nếu mô-đun chưa được cài đặt).</span><span class="sxs-lookup"><span data-stu-id="93f65-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="93f65-105">Để thực hiện việc này, hãy đi tới [quản lý AZURE AD bằng Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="93f65-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="93f65-106">Làm theo các bước trong phần "tình huống 1: AD FS mã thông báo ký chứng chỉ hết hạn" của ["đã có sự cố truy cập vào trang web" lỗi từ AD FS khi người dùng liên kết đăng nhập vào Microsoft 365, Azure hoặc InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="93f65-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="93f65-107">Làm theo các bước trong [bản Cập Nhật hoặc sửa chữa cài đặt của một liên kết miền trong Microsoft, Azure hoặc InTune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="93f65-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="93f65-108">Để tìm hiểu thêm về tái tạo chứng chỉ liên kết, hãy xem gia [hạn chứng chỉ liên kết cho Microsoft 365 và Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="93f65-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
