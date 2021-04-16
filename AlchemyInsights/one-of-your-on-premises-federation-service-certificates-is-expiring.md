---
title: Một trong số chứng chỉ dịch vụ liên kết tại cơ sở của bạn bị hết hạn
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810074"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="6849b-102">Một trong số chứng chỉ dịch vụ liên kết tại cơ sở của bạn bị hết hạn</span><span class="sxs-lookup"><span data-stu-id="6849b-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="6849b-103">Để giải quyết vấn đề này, hãy làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="6849b-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="6849b-104">Cài đặt mô-đun Microsoft Azure Active Directory cho Windows PowerShell trên máy tính (nếu mô-đun chưa được cài đặt).</span><span class="sxs-lookup"><span data-stu-id="6849b-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="6849b-105">Để thực hiện thao tác này, hãy đi đến [Azure Active Directory PowerShell cho đồ thị ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="6849b-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="6849b-106">Làm theo các bước trong "kịch bản 1: chứng chỉ ký mã hóa AD FS đã hết hạn" phần "của [" đã xảy ra sự cố khi truy nhập vào lỗi "site" từ AD FS khi một người dùng được liên kết đăng nhập vào Microsoft 365, Azure hoặc InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="6849b-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="6849b-107">Làm theo các bước trong [cách Cập Nhật hoặc sửa chữa các thiết đặt của tên miền được liên kết trong Microsoft 365, Azure hoặc InTune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="6849b-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="6849b-108">Để biết thêm thông tin về việc gia hạn chứng chỉ liên kết, hãy xem mục [chứng chỉ gia hạn cho O365 và AZURE AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="6849b-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

