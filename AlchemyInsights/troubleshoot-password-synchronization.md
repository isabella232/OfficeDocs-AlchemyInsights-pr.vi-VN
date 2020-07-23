---
title: Khắc phục sự cố đồng bộ hóa mật khẩu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387899"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="a732f-102">Khắc phục sự cố đồng bộ hóa mật khẩu</span><span class="sxs-lookup"><span data-stu-id="a732f-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="a732f-103">Để khắc phục sự cố đồng bộ hóa mật khẩu, khởi động bằng cách sử dụng công việc khắc phục sự cố AAD kết nối này để xác định lý do mật khẩu không đồng bộ hoá.</span><span class="sxs-lookup"><span data-stu-id="a732f-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="a732f-104">Để bắt đầu, hãy đi tới [quản lý đồng bộ trực tiếp](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="a732f-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="a732f-105">Mở phiên Windows PowerShell mới trên máy chủ Azure AD kết nối của bạn và chọn tuỳ chọn **chạy như quản trị viên** .</span><span class="sxs-lookup"><span data-stu-id="a732f-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="a732f-106">Chạy thiết lập ExecutionPolicy RemoteSigned hoặc Set-ExecutionPolicy không hạn chế.</span><span class="sxs-lookup"><span data-stu-id="a732f-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="a732f-107">Khởi động thuật sĩ Azure AD kết nối.</span><span class="sxs-lookup"><span data-stu-id="a732f-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="a732f-108">Truy cập trang tác vụ bổ sung > **khắc phục sự cố**  >  **tiếp theo**.</span><span class="sxs-lookup"><span data-stu-id="a732f-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="a732f-109">Chọn **khởi chạy** để mở menu khắc phục sự cố PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a732f-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="a732f-110">Chọn **khắc phục sự cố đồng bộ hóa mật khẩu**.</span><span class="sxs-lookup"><span data-stu-id="a732f-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="a732f-111">Vấn đề thường là mật khẩu không đồng bộ hoá tài khoản người dùng cụ thể.</span><span class="sxs-lookup"><span data-stu-id="a732f-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="a732f-112">**Ghi chú** Đồng bộ hóa mật khẩu không thành công nếu đồng bộ hoá mật khẩu thành công cuối cùng là một số thời gian trước đây.</span><span class="sxs-lookup"><span data-stu-id="a732f-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="a732f-113">Để được trợ giúp thêm khắc phục sự cố đồng bộ hóa mật khẩu, xem [khắc phục sự cố đồng bộ hóa mật khẩu băm AZURE AD kết nối đồng bộ](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="a732f-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>