---
title: Một trong những chứng chỉ dịch vụ liên kết tại chỗ của bạn hết hạn
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 24c369c61ad7cf7a9fe101ac29271c32e5159c1f
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761405"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="cf009-102">Một trong những chứng chỉ dịch vụ liên kết tại chỗ của bạn hết hạn</span><span class="sxs-lookup"><span data-stu-id="cf009-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="cf009-103">Để khắc phục sự cố này, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="cf009-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="cf009-104">Cài đặt Microsoft Azure Active Directory mô-đun Windows PowerShell trên máy tính (nếu mô-đun chưa được cài đặt).</span><span class="sxs-lookup"><span data-stu-id="cf009-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="cf009-105">Để thực hiện việc này, hãy truy cập [Azure Active Directory PowerShell cho đồ thị](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="cf009-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="cf009-106">Làm theo các bước trong phần "tình huống 1: AD FS mã thông báo ký chứng chỉ hết hạn" của ["đã có sự cố truy cập vào trang web" lỗi từ AD FS khi người dùng liên kết đăng nhập vào Office 365, Azure hoặc InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="cf009-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="cf009-107">Làm theo các bước trong t[làm thế nào để cập nhật hoặc sửa chữa các thiết đặt của một liên kết miền trong Office 365, Azure hoặc InTune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="cf009-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="cf009-108">Để biết thêm thông tin về đổi mới chứng chỉ liên kết, xem gia [hạn chứng chỉ O365 và AZURE AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="cf009-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

