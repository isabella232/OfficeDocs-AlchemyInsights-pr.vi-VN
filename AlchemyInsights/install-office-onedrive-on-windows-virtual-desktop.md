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
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Cài đặt Office và OneDrive trên máy tính chạy Windows ảo

1. [Chuẩn bị và tùy chỉnh ảnh VHD bản cái](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Tạo một máy ảo (VM) nếu nó chưa được tạo.

1. [Cài đặt Office trong chế độ kích hoạt máy tính dùng chung](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). Kích hoạt máy tính được chia sẻ cho phép nhiều người dùng truy nhập Office.

1. [Cài đặt OneDrive trong chế độ mỗi máy](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode). Thông thường, OneDrive được cài đặt cho mỗi người dùng, nhưng ở đây, cần phải cài đặt trên mỗi máy.