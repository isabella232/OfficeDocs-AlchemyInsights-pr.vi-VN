---
title: Mã lỗi 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Nếu bạn nhận được một lỗi trong khi kích hoạt Office 2013 trên dịch vụ máy tính để bàn từ xa (RDS) triển khai, hãy xem xét cho phép ADAL bằng cách chỉnh sửa registry.
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388267"
---
<span data-ttu-id="1d45d-103">Nếu bạn nhận được một lỗi trong khi kích hoạt Office 2013 trên dịch vụ máy tính để bàn từ xa (RDS) triển khai, hãy xem xét cho phép ADAL bằng cách chỉnh sửa registry.</span><span class="sxs-lookup"><span data-stu-id="1d45d-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="1d45d-104">**Khóa sổ đăng ký**</span><span class="sxs-lookup"><span data-stu-id="1d45d-104">**Registry key**</span></span>|<span data-ttu-id="1d45d-105">**Loại hình**</span><span class="sxs-lookup"><span data-stu-id="1d45d-105">**Type**</span></span>|<span data-ttu-id="1d45d-106">**Giá trị**</span><span class="sxs-lookup"><span data-stu-id="1d45d-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1d45d-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="1d45d-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="1d45d-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="1d45d-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="1d45d-109">1</span><span class="sxs-lookup"><span data-stu-id="1d45d-109">1</span></span>  <br/> |

<span data-ttu-id="1d45d-110">Để biết thêm chi tiết, hãy xem [Sử xác thực hiện đại cho Office 2013 trên thiết bị Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="1d45d-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="1d45d-111">ADAL được kích hoạt theo mặc định trong Office 365 ProPlus và Office 2016.</span><span class="sxs-lookup"><span data-stu-id="1d45d-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="1d45d-112">> dịch vụ máy tính để bàn từ xa (RDS) trước đây được đặt tên là dịch vụ đầu cuối.</span><span class="sxs-lookup"><span data-stu-id="1d45d-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  