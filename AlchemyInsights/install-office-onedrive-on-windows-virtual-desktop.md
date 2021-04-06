---
title: Cài đặt Office và OneDrive trên máy tính chạy Windows ảo
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596028"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="09954-102">Cài đặt Office và OneDrive trên máy tính chạy Windows ảo</span><span class="sxs-lookup"><span data-stu-id="09954-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="09954-103">[Chuẩn bị và tùy chỉnh ảnh VHD bản cái](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span><span class="sxs-lookup"><span data-stu-id="09954-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="09954-104">Tạo một máy ảo (VM) nếu nó chưa được tạo.</span><span class="sxs-lookup"><span data-stu-id="09954-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="09954-105">[Cài đặt Office trong chế độ kích hoạt máy tính dùng chung](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span><span class="sxs-lookup"><span data-stu-id="09954-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="09954-106">Kích hoạt máy tính được chia sẻ cho phép nhiều người dùng truy nhập Office.</span><span class="sxs-lookup"><span data-stu-id="09954-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="09954-107">[Cài đặt OneDrive trong chế độ mỗi máy](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span><span class="sxs-lookup"><span data-stu-id="09954-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="09954-108">Thông thường, OneDrive được cài đặt cho mỗi người dùng, nhưng ở đây, cần phải cài đặt trên mỗi máy.</span><span class="sxs-lookup"><span data-stu-id="09954-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>