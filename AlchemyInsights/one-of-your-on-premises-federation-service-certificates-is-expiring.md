---
title: Một trong số chứng chỉ dịch vụ liên kết tại cơ sở của bạn bị hết hạn
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673519"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="5ee87-102">Một trong số chứng chỉ dịch vụ liên kết tại cơ sở của bạn bị hết hạn</span><span class="sxs-lookup"><span data-stu-id="5ee87-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="5ee87-103">Để giải quyết vấn đề này, hãy làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="5ee87-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="5ee87-104">Cài đặt mô-đun Microsoft Azure Active Directory cho Windows PowerShell trên máy tính (nếu mô-đun chưa được cài đặt).</span><span class="sxs-lookup"><span data-stu-id="5ee87-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="5ee87-105">Để thực hiện thao tác này, hãy đi đến [Azure Active Directory PowerShell cho đồ thị ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="5ee87-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="5ee87-106">Làm theo các bước trong "kịch bản 1: chứng chỉ ký mã hóa AD FS đã hết hạn" phần "của [" đã xảy ra sự cố khi truy nhập vào lỗi "site" từ AD FS khi một người dùng được liên kết đăng nhập vào Microsoft 365, Azure hoặc InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="5ee87-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="5ee87-107">Làm theo các bước trong [cách Cập Nhật hoặc sửa chữa các thiết đặt của tên miền được liên kết trong Microsoft 365, Azure hoặc InTune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="5ee87-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="5ee87-108">Để biết thêm thông tin về việc gia hạn chứng chỉ liên kết, hãy xem mục [chứng chỉ gia hạn cho O365 và AZURE AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="5ee87-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

