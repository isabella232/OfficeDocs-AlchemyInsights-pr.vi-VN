---
title: Mã lỗi 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Nếu bạn gặp lỗi khi kích hoạt Office 2013 trên các triển khai dịch vụ máy tính để bàn từ xa (RDS), hãy xem xét cho phép ADAL bằng cách chỉnh sửa sổ đăng ký.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703160"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="b68ad-103">Lỗi khi kích hoạt Office 2013 trên máy tính để bàn từ xa dịch vụ</span><span class="sxs-lookup"><span data-stu-id="b68ad-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="b68ad-104">Nếu bạn gặp lỗi khi kích hoạt Office 2013 trên các triển khai dịch vụ máy tính để bàn từ xa (RDS), hãy xem xét cho phép ADAL bằng cách chỉnh sửa sổ đăng ký.</span><span class="sxs-lookup"><span data-stu-id="b68ad-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="b68ad-105">**Khoá đăng ký**</span><span class="sxs-lookup"><span data-stu-id="b68ad-105">**Registry key**</span></span>|<span data-ttu-id="b68ad-106">**Loại**</span><span class="sxs-lookup"><span data-stu-id="b68ad-106">**Type**</span></span>|<span data-ttu-id="b68ad-107">**Đáng giá tiền**</span><span class="sxs-lookup"><span data-stu-id="b68ad-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b68ad-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="b68ad-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="b68ad-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="b68ad-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="b68ad-110">1</span><span class="sxs-lookup"><span data-stu-id="b68ad-110">1</span></span>  <br/> |

<span data-ttu-id="b68ad-111">Để biết thêm thông tin, xem [kích hoạt xác thực hiện đại cho Office 2013 trên thiết bị Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="b68ad-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="b68ad-112">ADAL được bật theo mặc định trong Microsoft 365 ứng dụng cho doanh nghiệp và Office 2016.</span><span class="sxs-lookup"><span data-stu-id="b68ad-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="b68ad-113">Dịch vụ máy tính để bàn từ xa (RDS) trước đây có tên là dịch vụ đầu cuối.</span><span class="sxs-lookup"><span data-stu-id="b68ad-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  