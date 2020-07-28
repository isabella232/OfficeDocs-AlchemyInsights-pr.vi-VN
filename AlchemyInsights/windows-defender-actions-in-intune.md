---
title: Hành động của Windows Defender trong InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1282"
- "6700008"
ms.openlocfilehash: 61a2411ce7c4578ecf2c32943c6a21edbf63eeee
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440437"
---
# <a name="windows-defender-actions-in-intune"></a><span data-ttu-id="01e97-102">Hành động của Windows Defender trong InTune</span><span class="sxs-lookup"><span data-stu-id="01e97-102">Windows Defender actions in Intune</span></span>

<span data-ttu-id="01e97-103">InTune có thể được sử dụng để kích hoạt quét theo yêu cầu và Cập Nhật chữ ký vi rút cho Windows Defender trên các thiết bị riêng lẻ.</span><span class="sxs-lookup"><span data-stu-id="01e97-103">Intune can be used to trigger an on-demand scan and virus signature update for Windows Defender on individual devices.</span></span>

<span data-ttu-id="01e97-104">Sau khi một hành động từ xa được kích hoạt thành công hoạt động được phản ánh trong Nhật ký sự kiện Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="01e97-104">After a remote action is successfully triggered the activity is reflected in the Windows Defender event log.</span></span>

<span data-ttu-id="01e97-105">Chính sách bảo vệ điểm cuối của Windows cho phép các thiết đặt bổ sung cho các tính năng của Windows Defender được tạo ra trong InTune và áp dụng cho bộ thiết bị.</span><span class="sxs-lookup"><span data-stu-id="01e97-105">Windows Endpoint Protection policy allows additional settings for Windows Defender features to be created in Intune and applied to sets of devices.</span></span>

<span data-ttu-id="01e97-106">Để biết thêm chi tiết về kích hoạt các hành động của bộ bảo vệ Windows, xem [cấu hình và chạy quét chống vi-rút Microsoft Defender theo yêu cầu](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="01e97-106">For more details on triggering Windows Defender actions, see [Configure and run on-demand Microsoft Defender Antivirus scans](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span></span>