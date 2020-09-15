---
title: Tạm dừng Cập Nhật theo lịch trình
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 13abc7c9201b1897a9c766add4d105ef12f0d66f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721577"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="17d3e-102">Tạm dừng Cập Nhật theo lịch trình</span><span class="sxs-lookup"><span data-stu-id="17d3e-102">Pausing scheduled updates</span></span>

<span data-ttu-id="17d3e-103">Khi lệnh tạm dừng được phát hành, các thiết bị không xử lý lệnh cho đến lần tiếp theo, họ kiểm nhập vào InTune.</span><span class="sxs-lookup"><span data-stu-id="17d3e-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="17d3e-104">Vì điều này, các thiết bị của bạn có thể có:</span><span class="sxs-lookup"><span data-stu-id="17d3e-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="17d3e-105">Đã cài đặt các bản Cập Nhật được lên lịch trước khi kiểm nhập.</span><span class="sxs-lookup"><span data-stu-id="17d3e-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="17d3e-106">Được hỗ trợ khi bạn ban hành lệnh tạm dừng.</span><span class="sxs-lookup"><span data-stu-id="17d3e-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="17d3e-107">Trong trường hợp này, khi các thiết bị được hỗ trợ, họ có thể đã tải xuống và cài đặt các bản Cập Nhật được lên lịch trước khi kiểm nhập.</span><span class="sxs-lookup"><span data-stu-id="17d3e-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>