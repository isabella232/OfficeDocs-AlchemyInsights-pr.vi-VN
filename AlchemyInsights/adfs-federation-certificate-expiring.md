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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c9922258c2d203cc07c1a1055ffa36c23a756115
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36499913"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="6a69b-102">ADFS liên chứng chỉ hết hạn</span><span class="sxs-lookup"><span data-stu-id="6a69b-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="6a69b-103">Để giải quyết vấn đề này, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="6a69b-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="6a69b-104">Cài đặt các Microsoft Azure Active Directory Module cho Windows PowerShell trên máy tính (nếu các mô-đun đã không được cài đặt).</span><span class="sxs-lookup"><span data-stu-id="6a69b-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="6a69b-105">Để làm điều này, hãy [quản lý Azure quảng cáo bằng cách sử dụng Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="6a69b-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="6a69b-106">Làm theo các bước trong những "kịch bản 1: AD FS token-ký chứng chỉ hết hạn" phần ["Đã có một vấn đề khi truy cập các trang web"](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)lỗi từ AD FS khi người dùng đã liên kết đăng nhập Office 365, Azure, hoặc dành.</span><span class="sxs-lookup"><span data-stu-id="6a69b-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="6a69b-107">Làm theo các bước làm thế nào [để cập nhật hoặc sửa chữa cài đặt của một tên miền đã liên kết trong Office 365, Azure, hoặc dành](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="6a69b-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>

    <span data-ttu-id="6a69b-108">Để tìm hiểu thêm về đổi mới liên chứng chỉ, hãy xem [Renew liên chứng chỉ cho Office 365 và Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="6a69b-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
