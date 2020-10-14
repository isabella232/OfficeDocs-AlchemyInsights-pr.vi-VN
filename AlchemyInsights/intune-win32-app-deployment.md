---
title: Triển khai ứng dụng InTune Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461998"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="458a2-102">Triển khai ứng dụng InTune Win32</span><span class="sxs-lookup"><span data-stu-id="458a2-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="458a2-103">Microsoft InTune cho phép các ứng dụng Win32, bao gồm nhưng không giới hạn đối với MSI và. EXE sẽ được triển khai cho các thiết bị chạy Windows 10.</span><span class="sxs-lookup"><span data-stu-id="458a2-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="458a2-104">Cơ chế triển khai dùng yêu cầu phần mở rộng quản lý InTune (IME) sẽ được trình bày trên thiết bị đích.</span><span class="sxs-lookup"><span data-stu-id="458a2-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="458a2-105">IME sẽ được cài đặt tự động như là kết quả của việc nhắm vào một tập lệnh PowerShell hoặc triển khai ứng dụng Win32 cho người dùng/thiết bị.</span><span class="sxs-lookup"><span data-stu-id="458a2-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="458a2-106">Ngoài ra còn có một tập hợp các site Pre-requiphải được đáp ứng để triển khai các ứng dụng Win32, trong đó bao gồm:</span><span class="sxs-lookup"><span data-stu-id="458a2-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="458a2-107">Nền tảng được hỗ trợ: Windows 10 phiên bản 1607 trở lên (các phiên bản Enterprise, Pro và Education).</span><span class="sxs-lookup"><span data-stu-id="458a2-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="458a2-108">Kiến trúc được hỗ trợ: x86 và x64.</span><span class="sxs-lookup"><span data-stu-id="458a2-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="458a2-109">Quản lý thiết bị: đã tham gia và tự động đăng ký (bao gồm cả tên miền hỗn hợp gia nhập và tự động đăng ký cho chính sách Nhóm).</span><span class="sxs-lookup"><span data-stu-id="458a2-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="458a2-110">Định dạng gói ứng dụng:. tệp **intunewin**  được chuẩn bị bởi [công cụ Prep Microsoft Win32 Content](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="458a2-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="458a2-111">Ể</span><span class="sxs-lookup"><span data-stu-id="458a2-111">Limitations:</span></span>
    - <span data-ttu-id="458a2-112">Kích cỡ tối đa: 8GB.</span><span class="sxs-lookup"><span data-stu-id="458a2-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="458a2-113">Cấu trúc không được hỗ trợ: cánh tay.</span><span class="sxs-lookup"><span data-stu-id="458a2-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="458a2-114">Xem lại tài liệu "[Thêm, gán và theo dõi ứng dụng Win32 trong Microsoft InTune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" để biết thông tin liên quan đến các bước sau.</span><span class="sxs-lookup"><span data-stu-id="458a2-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="458a2-115">Chi tiết về khắc phục sự cố về triển khai ứng dụng trên Windows bao gồm các ứng dụng Win32 có thể được xem xét trong các tài liệu sau đây</span><span class="sxs-lookup"><span data-stu-id="458a2-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="458a2-116">Khắc phục sự cố cài đặt ứng dụng</span><span class="sxs-lookup"><span data-stu-id="458a2-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="458a2-117">Khắc phục sự cố ứng dụng Win32</span><span class="sxs-lookup"><span data-stu-id="458a2-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)