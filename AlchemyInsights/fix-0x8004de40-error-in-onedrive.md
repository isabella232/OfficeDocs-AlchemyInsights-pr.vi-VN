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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525081"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="4ebc9-102">Khắc phục lỗi 0x8004de40 trong OneDrive</span><span class="sxs-lookup"><span data-stu-id="4ebc9-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="4ebc9-103">Nếu bạn nhận được một lỗi 0x8004de40 với OneDrive:</span><span class="sxs-lookup"><span data-stu-id="4ebc9-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="4ebc9-104">Khởi động lại máy tính bị ảnh hưởng, trong khi kết nối với miền Acitve thư mục của bạn.</span><span class="sxs-lookup"><span data-stu-id="4ebc9-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="4ebc9-105">Nếu khởi động lại không giải quyết vấn đề, unjoin và quay trở lại điện thoại từ các quảng cáo Azure.</span><span class="sxs-lookup"><span data-stu-id="4ebc9-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="4ebc9-106">**Lưu ý**: bạn nên trên mạng doanh nghiệp của bạn trong khi thực hiện các bước sau.</span><span class="sxs-lookup"><span data-stu-id="4ebc9-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="4ebc9-107">Không thực hiện các bước sau khi bạn không thể kết nối với cơ sở hạ tầng công ty của bạn (ví dụ, trong khi đi du lịch).</span><span class="sxs-lookup"><span data-stu-id="4ebc9-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="4ebc9-108">Mở một dấu nhắc lệnh nâng lên.</span><span class="sxs-lookup"><span data-stu-id="4ebc9-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="4ebc9-109">Để mở một dấu nhắc lệnh cao, nhấp vào - **bắt đầu**, bấm chuột phải vào **dấu nhắc lệnh**và sau đó nhấp vào **chạy như quản trị**.</span><span class="sxs-lookup"><span data-stu-id="4ebc9-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="4ebc9-110">Nhập *dsregcmd /leave* và nhấn **Enter**.</span><span class="sxs-lookup"><span data-stu-id="4ebc9-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="4ebc9-111">Khi hoàn tất, nhập *dsregcmd /join* và nhấn **Enter**.</span><span class="sxs-lookup"><span data-stu-id="4ebc9-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="4ebc9-112">Khi hoàn thành, đóng dấu nhắc lệnh.</span><span class="sxs-lookup"><span data-stu-id="4ebc9-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="4ebc9-113">Khởi động lại máy tính và đăng nhập vào OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4ebc9-113">Reboot the computer, and log into OneDrive.</span></span>