---
title: Microsoft Edge đặt cấu hình thiết đặt quyền riêng tư
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678865"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="08959-102">Microsoft Edge đặt cấu hình thiết đặt quyền riêng tư</span><span class="sxs-lookup"><span data-stu-id="08959-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="08959-103">Theo mặc định, nếu Microsoft Edge được triển khai trên nền tảng không phải Windows, dữ liệu chẩn đoán và thông tin site sẽ không được gửi đến Microsoft.</span><span class="sxs-lookup"><span data-stu-id="08959-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="08959-104">Tuy nhiên, nếu Microsoft Edge được triển khai trên Windows 10, dữ liệu chẩn đoán và thông tin site được gửi theo [cài đặt dữ liệu chẩn đoán Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)của người dùng.</span><span class="sxs-lookup"><span data-stu-id="08959-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="08959-105">Để cấu hình cách Microsoft Edge xử lý thu thập dữ liệu cho tổ chức của bạn, hãy sử dụng các chính sách nhóm sau đây:</span><span class="sxs-lookup"><span data-stu-id="08959-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="08959-106">[Metricsreportingenabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): chính sách này cho phép báo cáo về việc sử dụng và dữ liệu liên quan đến sự cố.</span><span class="sxs-lookup"><span data-stu-id="08959-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="08959-107">[Sendsiteinfotoimproveservices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): chính sách này sẽ gửi thông tin site được dùng để cải thiện các dịch vụ của Microsoft.</span><span class="sxs-lookup"><span data-stu-id="08959-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="08959-108">Để tìm hiểu thêm, hãy xem [cấu hình thiết đặt chính sách](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="08959-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>