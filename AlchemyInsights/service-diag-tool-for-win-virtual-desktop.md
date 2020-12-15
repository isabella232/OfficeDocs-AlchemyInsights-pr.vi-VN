---
title: Công cụ chẩn đoán dịch vụ cho máy tính để bàn Windows ảo
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680237"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="6f76c-102">Công cụ chẩn đoán dịch vụ cho máy tính để bàn Windows ảo</span><span class="sxs-lookup"><span data-stu-id="6f76c-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="6f76c-103">Windows Virtual Desktop (WVD) cung cấp một công cụ chẩn đoán cho phép người quản trị xác định lỗi thông qua một giao diện duy nhất.</span><span class="sxs-lookup"><span data-stu-id="6f76c-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="6f76c-104">Công cụ này ghi lại thông tin liên quan đến chẩn đoán mọi khi WVD được người đã gán vai trò WVD.</span><span class="sxs-lookup"><span data-stu-id="6f76c-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="6f76c-105">Mỗi Nhật ký có chứa thông tin về vai trò WVD tham gia vào hoạt động này, các thông báo lỗi xuất hiện trong phiên làm việc và thông tin về đối tượng thuê và người dùng.</span><span class="sxs-lookup"><span data-stu-id="6f76c-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="6f76c-106">Phân tích Nhật ký Azure có thể được cấu hình để chụp Nhật ký hoạt động được tạo bởi công cụ chẩn đoán.</span><span class="sxs-lookup"><span data-stu-id="6f76c-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="6f76c-107">Dưới đây là cách thực hiện:</span><span class="sxs-lookup"><span data-stu-id="6f76c-107">Here's how:</span></span>

1. <span data-ttu-id="6f76c-108">Tạo không gian làm việc phân tích Nhật ký với [cổng thông tin Azure](https://go.microsoft.com/fwlink/?linkid=2129500) hoặc [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="6f76c-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="6f76c-109">[Kết nối máy tính Windows với Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="6f76c-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="6f76c-110">Lấy ID không gian làm việc và khóa chính của không gian làm việc của bạn.</span><span class="sxs-lookup"><span data-stu-id="6f76c-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="6f76c-111">Trình hướng dẫn thiết lập cần thông tin này để cấu hình đúng cho tác nhân và để đảm bảo nó có thể liên lạc với Azure theo dõi.</span><span class="sxs-lookup"><span data-stu-id="6f76c-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="6f76c-112">[Đẩy chẩn đoán dữ liệu đến không gian làm việc của bạn](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="6f76c-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="6f76c-113">Bạn có thể đẩy chẩn đoán dữ liệu từ đối tượng thuê WVD của mình vào phân tích Nhật ký cho không gian làm việc của bạn.</span><span class="sxs-lookup"><span data-stu-id="6f76c-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="6f76c-114">[Xác định và chẩn đoán](https://go.microsoft.com/fwlink/?linkid=2128338) các sự cố nằm bên trong hoặc bên ngoài liên quan đến wvd.</span><span class="sxs-lookup"><span data-stu-id="6f76c-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="6f76c-115">Để tìm hiểu thêm về việc cấu hình công cụ chẩn đoán dịch vụ cho WVD, hãy xem [dùng phân tích Nhật ký cho tính năng chẩn đoán](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="6f76c-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
