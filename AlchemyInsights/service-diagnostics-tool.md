---
title: Công cụ chẩn đoán dịch vụ cho máy tính để bàn Windows ảo
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596042"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="5db9a-102">Công cụ chẩn đoán dịch vụ cho máy tính để bàn Windows ảo</span><span class="sxs-lookup"><span data-stu-id="5db9a-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="5db9a-103">Windows Virtual Desktop (WVD) cung cấp một công cụ chẩn đoán cho phép người quản trị xác định lỗi thông qua một giao diện duy nhất.</span><span class="sxs-lookup"><span data-stu-id="5db9a-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="5db9a-104">Công cụ này ghi lại thông tin liên quan đến chẩn đoán mọi khi WVD được người đã gán vai trò WVD.</span><span class="sxs-lookup"><span data-stu-id="5db9a-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="5db9a-105">Mỗi Nhật ký có chứa thông tin về vai trò WVD tham gia vào hoạt động này, các thông báo lỗi xuất hiện trong phiên làm việc và thông tin về đối tượng thuê và người dùng.</span><span class="sxs-lookup"><span data-stu-id="5db9a-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="5db9a-106">Phân tích Nhật ký Azure có thể được cấu hình để chụp Nhật ký hoạt động được tạo bởi công cụ chẩn đoán bằng cách làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="5db9a-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="5db9a-107">Tạo không gian làm việc phân tích Nhật ký với [cổng thông tin Azure](https://go.microsoft.com/fwlink/?linkid=2129500) hoặc [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="5db9a-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="5db9a-108">[Kết nối máy tính Windows với Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="5db9a-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="5db9a-109">Lấy ID không gian làm việc và khóa chính của không gian làm việc của bạn.</span><span class="sxs-lookup"><span data-stu-id="5db9a-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="5db9a-110">Trình hướng dẫn thiết lập cần thông tin này để cấu hình đúng cho tác nhân và để đảm bảo nó có thể liên lạc với Azure theo dõi.</span><span class="sxs-lookup"><span data-stu-id="5db9a-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="5db9a-111">[Đẩy chẩn đoán dữ liệu đến không gian làm việc của bạn](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="5db9a-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="5db9a-112">Bạn có thể đẩy chẩn đoán dữ liệu từ đối tượng thuê WVD của mình vào phân tích Nhật ký cho không gian làm việc của bạn.</span><span class="sxs-lookup"><span data-stu-id="5db9a-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="5db9a-113">[Xác định và chẩn đoán](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) các sự cố nằm bên trong hoặc bên ngoài liên quan đến wvd.</span><span class="sxs-lookup"><span data-stu-id="5db9a-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="5db9a-114">Để tìm hiểu thêm về việc cấu hình công cụ chẩn đoán dịch vụ cho WVD, hãy xem dùng phân tích Nhật ký cho tính năng chẩn đoán.</span><span class="sxs-lookup"><span data-stu-id="5db9a-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>