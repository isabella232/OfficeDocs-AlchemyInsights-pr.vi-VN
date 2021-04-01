---
title: Đặt Microsoft Edge làm trình duyệt mặc định trên thiết bị đã tham gia tên miền
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491873"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="38c2f-102">Đặt Microsoft Edge làm trình duyệt mặc định trên thiết bị đã tham gia tên miền</span><span class="sxs-lookup"><span data-stu-id="38c2f-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="38c2f-103">Đặt Microsoft Edge làm trình duyệt mặc định:</span><span class="sxs-lookup"><span data-stu-id="38c2f-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="38c2f-104">[Tạo một tệp cấu hình liên kết mặc định](https://go.microsoft.com/fwlink/?linkid=2132437) và lưu trữ nó cục bộ hoặc trên một chia sẻ mạng.</span><span class="sxs-lookup"><span data-stu-id="38c2f-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="38c2f-105">Mở trình soạn thảo chính sách nhóm, rồi đi đến mẫu thiết bị quản trị **cấu hình máy tính**  >    >  **Windows**  >  **Explorer**.</span><span class="sxs-lookup"><span data-stu-id="38c2f-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="38c2f-106">Chọn **đặt một tệp cấu hình liên kết mặc định**.</span><span class="sxs-lookup"><span data-stu-id="38c2f-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="38c2f-107">Chọn **thiết đặt chính sách**, rồi chọn **bật**.</span><span class="sxs-lookup"><span data-stu-id="38c2f-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="38c2f-108">Bên dưới **tùy chọn**, hãy nhập vị trí của tệp cấu hình liên kết mặc định của bạn, rồi chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="38c2f-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
