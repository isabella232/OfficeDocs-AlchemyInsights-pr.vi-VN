---
title: Khắc phục lỗi 0x8004de40 trong OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133998"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="d4114-102">Khắc phục lỗi 0x8004de40 trong OneDrive</span><span class="sxs-lookup"><span data-stu-id="d4114-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="d4114-103">Nếu bạn nhận được một lỗi 0x8004de40 với OneDrive:</span><span class="sxs-lookup"><span data-stu-id="d4114-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="d4114-104">Khởi động lại máy tính bị ảnh hưởng, trong khi kết nối với miền Acitve thư mục của bạn.</span><span class="sxs-lookup"><span data-stu-id="d4114-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="d4114-105">Nếu khởi động lại không giải quyết vấn đề, unjoin và quay trở lại điện thoại từ các quảng cáo Azure.</span><span class="sxs-lookup"><span data-stu-id="d4114-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="d4114-106">**Lưu ý**: bạn nên trên mạng doanh nghiệp của bạn trong khi thực hiện các bước sau.</span><span class="sxs-lookup"><span data-stu-id="d4114-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="d4114-107">Không thực hiện các bước sau khi bạn không thể kết nối với cơ sở hạ tầng công ty của bạn (ví dụ, trong khi đi du lịch).</span><span class="sxs-lookup"><span data-stu-id="d4114-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="d4114-108">Mở một dấu nhắc lệnh nâng lên.</span><span class="sxs-lookup"><span data-stu-id="d4114-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="d4114-109">Để mở một dấu nhắc lệnh cao, nhấp vào - **bắt đầu**, bấm chuột phải vào **dấu nhắc lệnh**và sau đó nhấp vào **chạy như quản trị**.</span><span class="sxs-lookup"><span data-stu-id="d4114-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="d4114-110">Nhập *dsregcmd /leave* và nhấn **Enter**.</span><span class="sxs-lookup"><span data-stu-id="d4114-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="d4114-111">Khi hoàn tất, nhập *dsregcmd /join* và nhấn **Enter**.</span><span class="sxs-lookup"><span data-stu-id="d4114-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="d4114-112">Khi hoàn thành, đóng dấu nhắc lệnh.</span><span class="sxs-lookup"><span data-stu-id="d4114-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="d4114-113">Khởi động lại máy tính và đăng nhập vào OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d4114-113">Reboot the computer, and log into OneDrive.</span></span>