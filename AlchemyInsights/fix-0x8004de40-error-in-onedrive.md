---
title: Khắc phục lỗi 0x8004de40 trong OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755870"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="9d94c-102">Khắc phục lỗi 0x8004de40 trong OneDrive</span><span class="sxs-lookup"><span data-stu-id="9d94c-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="9d94c-103">Nếu bạn nhận được lỗi 0x8004de40 với OneDrive:</span><span class="sxs-lookup"><span data-stu-id="9d94c-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="9d94c-104">Khởi động lại máy tính bị ảnh hưởng trong khi kết nối với miền Acitve thư mục của bạn.</span><span class="sxs-lookup"><span data-stu-id="9d94c-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="9d94c-105">Nếu khởi động lại không khắc phục sự cố, hủy tham gia và kết nối lại thiết bị của bạn từ Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9d94c-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="9d94c-106">**Lưu ý**: bạn nên trên mạng công ty của bạn trong khi thực hiện các bước sau.</span><span class="sxs-lookup"><span data-stu-id="9d94c-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="9d94c-107">Không thực hiện các bước này khi bạn không thể kết nối với cơ sở hạ tầng doanh nghiệp của mình (ví dụ: khi đang đi du lịch).</span><span class="sxs-lookup"><span data-stu-id="9d94c-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="9d94c-108">Mở dấu nhắc lệnh nâng cao.</span><span class="sxs-lookup"><span data-stu-id="9d94c-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="9d94c-109">Để mở dấu nhắc lệnh nâng cao, bấm- **bắt đầu**, bấm chuột phải vào **dấu nhắc lệnh**, và sau đó nhấp vào **chạy như quản trị viên**.</span><span class="sxs-lookup"><span data-stu-id="9d94c-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="9d94c-110">Nhập *dsregcmd/để lại* và nhấn **Enter**.</span><span class="sxs-lookup"><span data-stu-id="9d94c-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="9d94c-111">Khi hoàn tất, nhập *dsregcmd/tham gia* và nhấn **Enter**.</span><span class="sxs-lookup"><span data-stu-id="9d94c-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="9d94c-112">Khi hoàn tất, đóng dấu nhắc lệnh.</span><span class="sxs-lookup"><span data-stu-id="9d94c-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="9d94c-113">Khởi động lại máy tính và đăng nhập vào OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9d94c-113">Reboot the computer, and log into OneDrive.</span></span>