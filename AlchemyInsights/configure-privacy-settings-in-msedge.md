---
title: Đặt cấu hình thiết đặt quyền riêng tư trong Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405727"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="e2f36-102">Đặt cấu hình thiết đặt quyền riêng tư trong Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="e2f36-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="e2f36-103">Theo mặc định, nếu Microsoft Edge được triển khai trên nền tảng không phải Windows, dữ liệu chẩn đoán và thông tin site không được gửi đến Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e2f36-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="e2f36-104">Tuy nhiên, nếu Microsoft Edge được triển khai trên Windows 10, dữ liệu chẩn đoán và thông tin site được gửi theo [cài đặt dữ liệu chẩn đoán Windows](https://go.microsoft.com/fwlink/?linkid=2132472)của người dùng.</span><span class="sxs-lookup"><span data-stu-id="e2f36-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="e2f36-105">Để cấu hình cách Microsoft Edge xử lý thu thập dữ liệu cho tổ chức của bạn, hãy sử dụng các chính sách nhóm sau đây:</span><span class="sxs-lookup"><span data-stu-id="e2f36-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="e2f36-106">Hàm [Metricsreportingenabled](https://go.microsoft.com/fwlink/?linkid=2132470) sẽ bật báo cáo về việc sử dụng và dữ liệu liên quan đến sự cố.</span><span class="sxs-lookup"><span data-stu-id="e2f36-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="e2f36-107">[Sendsiteinfotoimproveservices](https://go.microsoft.com/fwlink/?linkid=2132470) gửi thông tin site được sử dụng để cải thiện các dịch vụ của Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e2f36-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="e2f36-108">Để tìm hiểu thêm, hãy xem [cấu hình thiết đặt chính sách](https://go.microsoft.com/fwlink/?linkid=2132577).</span><span class="sxs-lookup"><span data-stu-id="e2f36-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
