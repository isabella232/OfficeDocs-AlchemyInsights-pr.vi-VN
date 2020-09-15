---
title: Khắc phục sự cố đồng bộ hóa mật khẩu
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
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664948"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="67052-102">Khắc phục sự cố đồng bộ hóa mật khẩu</span><span class="sxs-lookup"><span data-stu-id="67052-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="67052-103">Để khắc phục sự cố về đồng bộ hóa mật khẩu, hãy bắt đầu bằng cách sử dụng tác vụ khắc phục sự cố kết nối này để xác định tại sao mật khẩu không đồng bộ.</span><span class="sxs-lookup"><span data-stu-id="67052-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="67052-104">Để bắt đầu, hãy đi đến [quản lý đồng bộ trực tiếp](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="67052-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="67052-105">Mở phiên Windows PowerShell mới trên máy chủ Azure AD Connect của bạn, rồi chọn tùy chọn **chạy với tư cách người quản trị** .</span><span class="sxs-lookup"><span data-stu-id="67052-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="67052-106">Chạy Set-ExecutionPolicy RemoteSigned hoặc Set-ExecutionPolicy không hạn chế.</span><span class="sxs-lookup"><span data-stu-id="67052-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="67052-107">Khởi động trình hướng dẫn Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="67052-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="67052-108">Đi đến trang nhiệm vụ bổ sung > **khắc phục sự cố**  >  **tiếp theo**.</span><span class="sxs-lookup"><span data-stu-id="67052-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="67052-109">Chọn **khởi động** để mở menu khắc phục sự cố PowerShell.</span><span class="sxs-lookup"><span data-stu-id="67052-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="67052-110">Chọn **khắc phục sự cố đồng bộ hóa mật khẩu**.</span><span class="sxs-lookup"><span data-stu-id="67052-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="67052-111">Vấn đề thường là một mật khẩu không được đồng bộ cho một tài khoản người dùng cụ thể.</span><span class="sxs-lookup"><span data-stu-id="67052-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="67052-112">**Ghi chú** Đồng bộ hóa mật khẩu không thể nếu đồng bộ mật khẩu đã thành công cuối cùng đã được một thời gian trước đây.</span><span class="sxs-lookup"><span data-stu-id="67052-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="67052-113">Để biết thêm trợ giúp khắc phục sự cố đồng bộ hóa mật khẩu, hãy xem [khắc phục sự cố đồng bộ hóa băm mật khẩu với AZURE AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="67052-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>