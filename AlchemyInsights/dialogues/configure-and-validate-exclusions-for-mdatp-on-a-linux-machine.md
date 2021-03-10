---
title: Cấu hình và xác thực loại trừ cho MDATP trên máy Linux
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696075"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="8ff8f-102">Cấu hình và xác thực loại trừ cho MDATP trên máy Linux</span><span class="sxs-lookup"><span data-stu-id="8ff8f-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="8ff8f-103">Bạn có thể loại trừ các tệp nhất định, thư mục, quy trình và các tệp mở quá trình từ quét MDATP.</span><span class="sxs-lookup"><span data-stu-id="8ff8f-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="8ff8f-104">Việc loại trừ giúp tránh phát hiện không chính xác các phần mềm và tệp riêng biệt hoặc tùy chỉnh cho tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="8ff8f-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="8ff8f-105">Việc loại trừ cũng giúp giảm thiểu các vấn đề về hiệu suất do MDATP gây ra.</span><span class="sxs-lookup"><span data-stu-id="8ff8f-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="8ff8f-106">Để tìm hiểu thêm, hãy xem [cấu hình và xác thực các loại trừ cho MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="8ff8f-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="8ff8f-107">Các loại trừ được mô tả trong bài viết này không áp dụng cho các chức năng khác của MDATP for Linux, bao gồm Endpoint Detection and Response (EDR).</span><span class="sxs-lookup"><span data-stu-id="8ff8f-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="8ff8f-108">Các tệp mà bạn loại trừ bằng cách sử dụng các phương pháp được mô tả trong bài viết này vẫn có thể kích hoạt cảnh báo EDR và các chức năng phát hiện khác.</span><span class="sxs-lookup"><span data-stu-id="8ff8f-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
