---
title: Khắc phục sự cố cài đặt MDATP trên máy Mac
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749763"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="531a5-102">Khắc phục sự cố cài đặt MDATP trên máy Mac</span><span class="sxs-lookup"><span data-stu-id="531a5-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="531a5-103">Nếu cài đặt thủ công không thành công, trang **tóm tắt** của trình hướng dẫn cài đặt sẽ hiển thị lỗi sau:</span><span class="sxs-lookup"><span data-stu-id="531a5-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="531a5-104">Lỗi "đã xảy ra trong quá trình cài đặt.</span><span class="sxs-lookup"><span data-stu-id="531a5-104">"An error occurred during installation.</span></span> <span data-ttu-id="531a5-105">Trình cài đặt gặp phải lỗi khiến quá trình cài đặt không thành công.</span><span class="sxs-lookup"><span data-stu-id="531a5-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="531a5-106">Liên hệ với nhà sản xuất phần mềm để được trợ giúp. "</span><span class="sxs-lookup"><span data-stu-id="531a5-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="531a5-107">Đối với triển khai MDM, trang sẽ hiển thị lỗi cài đặt chung.</span><span class="sxs-lookup"><span data-stu-id="531a5-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="531a5-108">Mặc dù chúng tôi không hiển thị các lỗi chính xác cho người dùng cuối, chúng tôi giữ một tệp nhật ký với tiến trình cài đặt, trong **/Library/logs/Microsoft/mdatp/install.log**.</span><span class="sxs-lookup"><span data-stu-id="531a5-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="531a5-109">Mỗi phiên cài đặt sẽ nối vào tệp nhật ký này.</span><span class="sxs-lookup"><span data-stu-id="531a5-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="531a5-110">Để chỉ ra phiên cài đặt cuối cùng, hãy sử dụng `sed` .</span><span class="sxs-lookup"><span data-stu-id="531a5-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="531a5-111">Để tìm hiểu thêm, hãy xem [khắc phục sự cố cài đặt cho Microsoft Defender ATP cho Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="531a5-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
