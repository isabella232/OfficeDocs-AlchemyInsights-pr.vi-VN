---
title: Mã lỗi 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Nếu bạn nhận được một lỗi trong khi kích hoạt Office 2013 trên dịch vụ máy tính để bàn từ xa (RDS) triển khai, hãy xem xét cho phép ADAL bằng cách chỉnh sửa registry.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28320647"
---
<span data-ttu-id="28c9c-103">Nếu bạn nhận được một lỗi trong khi kích hoạt Office 2013 trên dịch vụ máy tính để bàn từ xa (RDS) triển khai, hãy xem xét cho phép ADAL bằng cách chỉnh sửa registry.</span><span class="sxs-lookup"><span data-stu-id="28c9c-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="28c9c-104">**Khóa sổ đăng ký**</span><span class="sxs-lookup"><span data-stu-id="28c9c-104">**Registry key**</span></span>|<span data-ttu-id="28c9c-105">\*\*Nhập \*\*</span><span class="sxs-lookup"><span data-stu-id="28c9c-105">**Type**</span></span>|<span data-ttu-id="28c9c-106">**Giá trị**</span><span class="sxs-lookup"><span data-stu-id="28c9c-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="28c9c-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="28c9c-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="28c9c-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="28c9c-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="28c9c-109">1</span><span class="sxs-lookup"><span data-stu-id="28c9c-109">1</span></span>  <br/> |
   
<span data-ttu-id="28c9c-110">Để biết thêm chi tiết, hãy xem [Sử xác thực hiện đại cho Office 2013 trên thiết bị Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="28c9c-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="28c9c-p101">ADAL được kích hoạt theo mặc định trong Office 365 ProPlus và Office 2016. > Dịch vụ từ xa máy tính để bàn (RDS) trước đây được đặt tên là dịch vụ đầu cuối.</span><span class="sxs-lookup"><span data-stu-id="28c9c-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

