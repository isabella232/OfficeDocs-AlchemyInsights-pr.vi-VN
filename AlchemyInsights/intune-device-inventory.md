---
title: Kiểm kê thiết bị InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667900"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="71a25-102">Kiểm kê thiết bị InTune</span><span class="sxs-lookup"><span data-stu-id="71a25-102">Intune Device Inventory</span></span>

<span data-ttu-id="71a25-103">Blade thiết bị cung cấp cho người quản trị hiểu sâu vào các thiết bị dưới quản lý trong InTune trên mỗi cơ sở thiết bị.</span><span class="sxs-lookup"><span data-stu-id="71a25-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="71a25-104">Thông tin được hiển thị bao gồm: phần cứng, ứng dụng đã phát hiện, trạng thái tuân thủ thiết bị và trạng thái cấu hình thiết bị.</span><span class="sxs-lookup"><span data-stu-id="71a25-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="71a25-105">Dữ liệu hàng tồn kho cho phần cứng và các ứng dụng được phát hiện được thu thập trong vòng tròn bảy ngày.</span><span class="sxs-lookup"><span data-stu-id="71a25-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="71a25-106">Các ứng dụng và phần cứng cụ thể được báo cáo khác nhau tùy thuộc vào hệ điều hành thiết bị và liệu thiết bị có cá nhân hoặc công ty thuộc sở hữu.</span><span class="sxs-lookup"><span data-stu-id="71a25-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="71a25-107">Để biết thêm thông tin, hãy xem [xem chi tiết thiết bị trong InTune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="71a25-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="71a25-108">**DIỄN**</span><span class="sxs-lookup"><span data-stu-id="71a25-108">**FAQ**</span></span>

<span data-ttu-id="71a25-109">Hỏi: tôi không nhận được danh sách các ứng dụng hàng tồn kho đầy đủ trình bày trên thiết bị Windows được đăng ký theo dõi.</span><span class="sxs-lookup"><span data-stu-id="71a25-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="71a25-110">Tại sao không?</span><span class="sxs-lookup"><span data-stu-id="71a25-110">Why not?</span></span>

<span data-ttu-id="71a25-111">A: tại thời điểm này, chỉ các ứng dụng hiện đại được liệt kê cho PC chạy Windows 10 được xác định là các thiết bị công ty.</span><span class="sxs-lookup"><span data-stu-id="71a25-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="71a25-112">InTune không thu thập thông tin về các ứng dụng Win32 được cài đặt trên các thiết bị này.</span><span class="sxs-lookup"><span data-stu-id="71a25-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="71a25-113">Hỏi: tại sao số điện thoại không được thu thập từ tất cả các thiết bị?</span><span class="sxs-lookup"><span data-stu-id="71a25-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="71a25-114">A: điện thoại được phân loại là các thiết bị công ty trong InTune không được xác định bằng số điện thoại đầy đủ của họ khi, ví dụ: bạn chạy báo cáo kiểm kê trên thiết bị di động.</span><span class="sxs-lookup"><span data-stu-id="71a25-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="71a25-115">Mang theo-bạn-riêng-các số điện thoại của thiết bị luôn là một phần masked với các dấu sao (\* \* \* \*) và chỉ hiện bốn chữ số cuối cùng.</span><span class="sxs-lookup"><span data-stu-id="71a25-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>