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
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745152"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="a5373-102">Khắc phục lỗi 0x8005de40 trong OneDrive</span><span class="sxs-lookup"><span data-stu-id="a5373-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="a5373-103">Nếu bạn nhận được lỗi 0x8005de40 với OneDrive:</span><span class="sxs-lookup"><span data-stu-id="a5373-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="a5373-104">Khởi động lại máy tính bị ảnh hưởng khi đã kết nối với tên miền Acitve Directory của bạn.</span><span class="sxs-lookup"><span data-stu-id="a5373-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="a5373-105">Nếu khởi động lại không khắc phục sự cố, hãy bỏ tham gia và gia nhập lại thiết bị của bạn từ Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a5373-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="a5373-106">**Lưu ý**: bạn nên có trong mạng công ty của bạn trong khi thực hiện các bước này.</span><span class="sxs-lookup"><span data-stu-id="a5373-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="a5373-107">Không thực hiện các bước này khi bạn không thể kết nối với cơ sở hạ tầng công ty của bạn (ví dụ, trong khi đang đi du lịch).</span><span class="sxs-lookup"><span data-stu-id="a5373-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="a5373-108">Mở một dấu nhắc lệnh nâng cao.</span><span class="sxs-lookup"><span data-stu-id="a5373-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="a5373-109">Để mở dấu nhắc lệnh nâng cao, hãy bấm vào **bắt đầu**, bấm chuột phải vào **dấu nhắc lệnh**, rồi bấm vào **chạy với tư cách là người quản trị**.</span><span class="sxs-lookup"><span data-stu-id="a5373-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="a5373-110">Nhập *dsregcmd/Leave* và nhấn **Enter**.</span><span class="sxs-lookup"><span data-stu-id="a5373-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="a5373-111">Khi hoàn thành, nhập *dsregcmd/join* và nhấn **Enter**.</span><span class="sxs-lookup"><span data-stu-id="a5373-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="a5373-112">Khi hoàn thành, hãy đóng dấu nhắc lệnh.</span><span class="sxs-lookup"><span data-stu-id="a5373-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="a5373-113">Khởi động lại máy tính và đăng nhập vào OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a5373-113">Reboot the computer, and log into OneDrive.</span></span>