---
title: lỗi 0x8006de40 khi khởi chạy OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813674"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="b96fe-102">lỗi 0x8006de40 khi khởi chạy OneDrive</span><span class="sxs-lookup"><span data-stu-id="b96fe-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="b96fe-103">Nếu bạn nhận được lỗi **0x8005de40** khi đăng nhập vào OneDrive, hãy khởi động lại máy tính khi kết nối với tên miền cơ quan hoặc trường học của bạn.</span><span class="sxs-lookup"><span data-stu-id="b96fe-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="b96fe-104">Nếu bạn nhận được lỗi này sau khi khởi động lại, hãy thử điều này khi được kết nối với tên miền cơ quan hoặc trường học của bạn:</span><span class="sxs-lookup"><span data-stu-id="b96fe-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="b96fe-105">Bấm vào bắt đầu, rồi nhập **CMD** hoặc **Command Prompt**  vào hộp tìm kiếm, bấm chuột phải vào ứng dụng nhắc lệnh, rồi chọn  **chạy với tư trình quản trị**.</span><span class="sxs-lookup"><span data-stu-id="b96fe-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="b96fe-106">Nếu bạn được nhắc nhập mật khẩu người quản trị hoặc để xác nhận, hãy nhập mật khẩu hoặc bấm **cho phép**.</span><span class="sxs-lookup"><span data-stu-id="b96fe-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="b96fe-107">Trong cửa sổ dấu nhắc lệnh, nhập **dsregcmd/Leave**  và wait cho lệnh để hoàn thành.</span><span class="sxs-lookup"><span data-stu-id="b96fe-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="b96fe-108">Sau đó, nhập **dsregcmd/join** và chờ lệnh để hoàn thành.</span><span class="sxs-lookup"><span data-stu-id="b96fe-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="b96fe-109">Khởi động lại máy tính của bạn.</span><span class="sxs-lookup"><span data-stu-id="b96fe-109">Reboot your computer.</span></span>
