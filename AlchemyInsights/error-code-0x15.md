---
title: Mã lỗi 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Nếu bạn nhận được lỗi trong khi kích hoạt Office 2013 về triển khai dịch vụ trên máy tính từ xa (RDS), hãy cân nhắc việc bật ADAL bằng cách chỉnh sửa sổ đăng ký.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709209"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="07210-103">Lỗi trong khi kích hoạt Office 2013 trên máy tính từ xa dịch vụ</span><span class="sxs-lookup"><span data-stu-id="07210-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="07210-104">Nếu bạn nhận được lỗi trong khi kích hoạt Office 2013 về triển khai dịch vụ trên máy tính từ xa (RDS), hãy cân nhắc việc bật ADAL bằng cách chỉnh sửa sổ đăng ký.</span><span class="sxs-lookup"><span data-stu-id="07210-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="07210-105">**Khóa sổ đăng ký**</span><span class="sxs-lookup"><span data-stu-id="07210-105">**Registry key**</span></span>|<span data-ttu-id="07210-106">**Kiểu**</span><span class="sxs-lookup"><span data-stu-id="07210-106">**Type**</span></span>|<span data-ttu-id="07210-107">**Đáng**</span><span class="sxs-lookup"><span data-stu-id="07210-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="07210-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="07210-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="07210-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="07210-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="07210-110">1</span><span class="sxs-lookup"><span data-stu-id="07210-110">1</span></span>  <br/> |

<span data-ttu-id="07210-111">Để biết thêm thông tin, hãy xem [bật xác thực hiện đại cho Office 2013 trên các thiết bị chạy Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="07210-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="07210-112">ADAL được bật theo mặc định trong các ứng dụng Microsoft 365 dành cho doanh nghiệp và Office 2016.</span><span class="sxs-lookup"><span data-stu-id="07210-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="07210-113">Dịch vụ trên máy tính từ xa (RDS) trước đây đã có tên là dịch vụ Terminal.</span><span class="sxs-lookup"><span data-stu-id="07210-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  