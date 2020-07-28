---
title: Kho thiết bị InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440482"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="06e85-102">Kho thiết bị InTune</span><span class="sxs-lookup"><span data-stu-id="06e85-102">Intune Device Inventory</span></span>

<span data-ttu-id="06e85-103">Thiết bị Blade cung cấp thông tin chi tiết quản trị viên vào thiết bị quản lý trong InTune trên cơ sở mỗi thiết bị.</span><span class="sxs-lookup"><span data-stu-id="06e85-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="06e85-104">Thông tin hiển thị bao gồm: phần cứng, phát hiện các ứng dụng, trạng thái tuân thủ thiết bị và trạng thái cấu hình thiết bị.</span><span class="sxs-lookup"><span data-stu-id="06e85-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="06e85-105">Kiểm kê dữ liệu cho phần cứng và phát hiện các ứng dụng được thu thập trên một chu kỳ bảy ngày.</span><span class="sxs-lookup"><span data-stu-id="06e85-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="06e85-106">Các ứng dụng và các yếu tố cụ thể của phần cứng báo cáo khác nhau tùy thuộc vào hệ điều hành thiết bị và cho dù thiết bị là cá nhân hoặc công ty sở hữu.</span><span class="sxs-lookup"><span data-stu-id="06e85-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="06e85-107">Để biết thêm thông tin, xem [xem chi tiết thiết bị trong InTune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="06e85-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="06e85-108">**Faq**</span><span class="sxs-lookup"><span data-stu-id="06e85-108">**FAQ**</span></span>

<span data-ttu-id="06e85-109">Câu hỏi: tôi không nhận được danh sách đầy đủ các ứng dụng hiện có trên các thiết bị Windows được đăng ký InTune.</span><span class="sxs-lookup"><span data-stu-id="06e85-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="06e85-110">Tại sao không?</span><span class="sxs-lookup"><span data-stu-id="06e85-110">Why not?</span></span>

<span data-ttu-id="06e85-111">A: tại thời gian này, chỉ các ứng dụng hiện đại được liệt kê cho PC chạy Windows 10 được xác định là thiết bị của doanh nghiệp.</span><span class="sxs-lookup"><span data-stu-id="06e85-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="06e85-112">InTune không thu thập thông tin về các ứng dụng Win32 cài đặt trên các thiết bị này.</span><span class="sxs-lookup"><span data-stu-id="06e85-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="06e85-113">Câu hỏi: tại sao các số điện thoại không được thu thập từ tất cả các thiết bị?</span><span class="sxs-lookup"><span data-stu-id="06e85-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="06e85-114">A: điện thoại phân loại là các thiết bị doanh nghiệp trong InTune không được xác định với số điện thoại đầy đủ của họ khi, ví dụ: bạn chạy báo cáo kho thiết bị di động.</span><span class="sxs-lookup"><span data-stu-id="06e85-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="06e85-115">Mang theo-bạn-số điện thoại riêng của thiết bị luôn được che khuất một phần bằng dấu hoa thị (\* \* \* \*), và chỉ thể hiện bốn chữ số cuối cùng.</span><span class="sxs-lookup"><span data-stu-id="06e85-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>