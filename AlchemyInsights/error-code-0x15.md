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
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527099"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="31fce-103">Lỗi khi kích hoạt Office 2013 trên dịch vụ máy tính để bàn từ xa</span><span class="sxs-lookup"><span data-stu-id="31fce-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="31fce-104">Nếu bạn nhận được một lỗi trong khi kích hoạt Office 2013 trên dịch vụ máy tính để bàn từ xa (RDS) triển khai, hãy xem xét cho phép ADAL bằng cách chỉnh sửa registry.</span><span class="sxs-lookup"><span data-stu-id="31fce-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="31fce-105">**Khóa sổ đăng ký**</span><span class="sxs-lookup"><span data-stu-id="31fce-105">**Registry key**</span></span>|<span data-ttu-id="31fce-106">**Loại hình**</span><span class="sxs-lookup"><span data-stu-id="31fce-106">**Type**</span></span>|<span data-ttu-id="31fce-107">**Giá trị**</span><span class="sxs-lookup"><span data-stu-id="31fce-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="31fce-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="31fce-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="31fce-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="31fce-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="31fce-110">1</span><span class="sxs-lookup"><span data-stu-id="31fce-110">1</span></span>  <br/> |

<span data-ttu-id="31fce-111">Để biết thêm chi tiết, hãy xem [Sử xác thực hiện đại cho Office 2013 trên thiết bị Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="31fce-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="31fce-112">ADAL được kích hoạt theo mặc định trong Office 365 ProPlus và Office 2016.</span><span class="sxs-lookup"><span data-stu-id="31fce-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="31fce-113">Dịch vụ máy tính để bàn từ xa (RDS) trước đây được đặt tên là dịch vụ đầu cuối.</span><span class="sxs-lookup"><span data-stu-id="31fce-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  