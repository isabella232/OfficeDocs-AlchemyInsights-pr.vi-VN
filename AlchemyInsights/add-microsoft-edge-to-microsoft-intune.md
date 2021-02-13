---
title: Thêm Microsoft Edge vào Microsoft InTune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194581"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="1682f-102">Thêm Microsoft Edge vào Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="1682f-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="1682f-103">Để có thể triển khai, cấu hình, giám sát và bảo vệ Microsoft Edge for Windows 10, trước tiên bạn phải thêm nó vào Microsoft InTune.</span><span class="sxs-lookup"><span data-stu-id="1682f-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="1682f-104">InTune hỗ trợ Microsoft Edge 77 và các phiên bản mới hơn.</span><span class="sxs-lookup"><span data-stu-id="1682f-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="1682f-105">InTune sẽ phát hiện bất kỳ bản cài đặt nào sẵn có của Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="1682f-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="1682f-106">Nếu Microsoft Edge được cài đặt trong ngữ cảnh người dùng, một bản cài đặt hệ thống sẽ ghi đè lên bản cài đặt trong ngữ cảnh người dùng.</span><span class="sxs-lookup"><span data-stu-id="1682f-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="1682f-107">Nếu Microsoft Edge được cài đặt trong ngữ cảnh hệ thống, thành công cài đặt sẽ được báo cáo.</span><span class="sxs-lookup"><span data-stu-id="1682f-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="1682f-108">Microsoft Edge 77 và các phiên bản mới hơn, cho tất cả các kênh trong ngữ cảnh người dùng, sẽ được ghi đè với Microsoft Edge được cài đặt trong ngữ cảnh hệ thống.</span><span class="sxs-lookup"><span data-stu-id="1682f-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="1682f-109">**Kiện**</span><span class="sxs-lookup"><span data-stu-id="1682f-109">**Prerequisite**</span></span>

<span data-ttu-id="1682f-110">Windows 10 phiên bản 1709 hoặc phiên bản mới hơn</span><span class="sxs-lookup"><span data-stu-id="1682f-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="1682f-111">**Các bước để thêm cạnh để InTune**</span><span class="sxs-lookup"><span data-stu-id="1682f-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="1682f-112">[Cấu hình ứng dụng trong InTune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="1682f-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="1682f-113">[Đặt cấu hình thông tin ứng dụng](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="1682f-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="1682f-114">[Cấu hình các thiết đặt ứng dụng](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="1682f-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="1682f-115">[Chọn các thẻ phạm vi (tùy chọn)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="1682f-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="1682f-116">[Thêm ứng dụng](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="1682f-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="1682f-117">Để được trợ giúp thêm, hãy xem [khắc phục sự cố](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="1682f-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




