---
title: Xác định các sự cố của Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596039"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="39d65-102">Xác định các sự cố của Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="39d65-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="39d65-103">Windows Virtual Desktop Diagnostics chỉ sử dụng một lệnh ghép ngắn PowerShell nhưng chứa nhiều tham số tùy chọn để giúp thu hẹp và cô lập các vấn đề.</span><span class="sxs-lookup"><span data-stu-id="39d65-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="39d65-104">Để bắt đầu:</span><span class="sxs-lookup"><span data-stu-id="39d65-104">To get started:</span></span> 

1. <span data-ttu-id="39d65-105">Tải xuống và nhập mô-đun Windows Virtual Desktop PowerShell.</span><span class="sxs-lookup"><span data-stu-id="39d65-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="39d65-106">Để biết chi tiết, hãy xem các [lệnh ghép ngắn trên máy tính chạy Windows ảo cho Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span><span class="sxs-lookup"><span data-stu-id="39d65-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="39d65-107">Chạy lệnh ghép ngắn sau đây để đăng nhập vào tài khoản của bạn:</span><span class="sxs-lookup"><span data-stu-id="39d65-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="39d65-108">Mẫu `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="39d65-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="39d65-109">**Lưu ý:** Tất cả các truy vấn bằng PowerShell phải bao gồm các tham số-tên người dùng hoặc-ActivityID.</span><span class="sxs-lookup"><span data-stu-id="39d65-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="39d65-110">Để biết các chức năng giám sát, hãy xem dùng [phân tích Nhật ký cho tính năng chẩn đoán](https://go.microsoft.com/fwlink/?linkid=2126847).</span><span class="sxs-lookup"><span data-stu-id="39d65-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="39d65-111">Để lọc các hoạt động chẩn đoán theo người dùng, hãy chạy lệnh ghép ngắn sau đây:</span><span class="sxs-lookup"><span data-stu-id="39d65-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="39d65-112">Mẫu `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="39d65-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="39d65-113">Có một danh sách các bộ lọc mà bạn có thể chạy để chẩn đoán vấn đề.</span><span class="sxs-lookup"><span data-stu-id="39d65-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="39d65-114">Để tìm hiểu thêm về các vấn đề về chẩn đoán, hãy xem [xác định và chẩn đoán sự cố của Windows Virtual trên máy tính bàn](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="39d65-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="39d65-115">Để tìm hiểu thêm về các lỗi phổ biến, hãy xem các [lỗi thường gặp trong senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="39d65-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
