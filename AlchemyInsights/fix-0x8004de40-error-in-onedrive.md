---
title: Khắc phục lỗi 0x8005de40 trong OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649770"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="017fc-102">Khắc phục lỗi 0x8005de40 trong OneDrive</span><span class="sxs-lookup"><span data-stu-id="017fc-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="017fc-103">Nếu bạn đang chạy Windows 7 và nhận được thông báo lỗi này, hãy [Cập Nhật để bật tls 1,1 và tls 1,2 là các giao thức bảo mật mặc định trong WinHTTP trong Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span><span class="sxs-lookup"><span data-stu-id="017fc-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="017fc-104">Nếu bạn đang chạy Windows 10 và bạn nhận được lỗi 0x8005de40 với OneDrive:</span><span class="sxs-lookup"><span data-stu-id="017fc-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="017fc-105">Khởi động lại máy tính bị ảnh hưởng khi đã kết nối với tên miền Acitve Directory của bạn.</span><span class="sxs-lookup"><span data-stu-id="017fc-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="017fc-106">Nếu khởi động lại không khắc phục sự cố, hãy bỏ tham gia và gia nhập lại thiết bị của bạn từ Azure AD.</span><span class="sxs-lookup"><span data-stu-id="017fc-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="017fc-107">**Lưu ý**: bạn nên có trong mạng công ty của bạn trong khi thực hiện các bước này.</span><span class="sxs-lookup"><span data-stu-id="017fc-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="017fc-108">Không thực hiện các bước này khi bạn không được kết nối với cơ sở hạ tầng công ty của bạn (ví dụ, trong khi đang đi du lịch).</span><span class="sxs-lookup"><span data-stu-id="017fc-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="017fc-109">Mở dấu nhắc lệnh nâng cao bằng cách chọn **bắt đầu**, bấm chuột phải vào **dấu nhắc lệnh**, rồi chọn **chạy với tư cách là người quản trị**.</span><span class="sxs-lookup"><span data-stu-id="017fc-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="017fc-110">Nhập *dsregcmd/Leave* và nhấn **Enter**.</span><span class="sxs-lookup"><span data-stu-id="017fc-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="017fc-111">Khi hoàn thành, nhập *dsregcmd/join* và nhấn **Enter**.</span><span class="sxs-lookup"><span data-stu-id="017fc-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="017fc-112">Khi hoàn thành, hãy đóng dấu nhắc lệnh.</span><span class="sxs-lookup"><span data-stu-id="017fc-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="017fc-113">Khởi động lại máy tính và đăng nhập vào OneDrive.</span><span class="sxs-lookup"><span data-stu-id="017fc-113">Reboot the computer, and log into OneDrive.</span></span>