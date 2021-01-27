---
title: Xóa hoặc khôi phục các ứng dụng
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015023"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="b920c-102">Xóa hoặc khôi phục các ứng dụng</span><span class="sxs-lookup"><span data-stu-id="b920c-102">Delete or restore applications</span></span>

<span data-ttu-id="b920c-103">**Để xóa một ứng dụng khỏi AZURE AD đối tượng thuê của bạn**:</span><span class="sxs-lookup"><span data-stu-id="b920c-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="b920c-104">Trong **cổng thông tin AZURE AD**, chọn **ứng dụng doanh nghiệp**.</span><span class="sxs-lookup"><span data-stu-id="b920c-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="b920c-105">Sau đó tìm và chọn ứng dụng mà bạn muốn xóa bỏ.</span><span class="sxs-lookup"><span data-stu-id="b920c-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="b920c-106">Trong phần **quản lý** trong ngăn bên trái, hãy chọn **thuộc tính**.</span><span class="sxs-lookup"><span data-stu-id="b920c-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="b920c-107">Chọn **xóa**, rồi chọn **có** để xác nhận bạn muốn xóa ứng dụng khỏi Azure AD đối tượng thuê của bạn.</span><span class="sxs-lookup"><span data-stu-id="b920c-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="b920c-108">Để biết thêm thông tin về cách xóa ứng dụng, hãy xem [bắt đầu nhanh: xóa một ứng dụng từ đối tượng thuê Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="b920c-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="b920c-109">Trong PowerShell, lệnh ghép ngắn [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) sẽ loại bỏ cấu hình proxy ứng dụng từ một ứng dụng cụ thể trong Azure Active Directory và có thể xóa ứng dụng hoàn toàn nếu được chỉ định.</span><span class="sxs-lookup"><span data-stu-id="b920c-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="b920c-110">Bạn có thể **khôi phục một ứng dụng đã xóa** bằng PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b920c-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="b920c-111">Sau khi ứng dụng mà bạn muốn khôi phục đã được xác định, bạn có thể khôi phục nó bằng cách dùng [khôi phục-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="b920c-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
