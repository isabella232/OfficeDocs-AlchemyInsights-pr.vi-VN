---
title: Microsoft Edge cấu hình thiết đặt quyền riêng tư
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
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114194"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge cấu hình thiết đặt quyền riêng tư

Theo mặc định, nếu Microsoft Edge triển khai trên các nền tảng không phải định dạng Windows, dữ liệu chẩn đoán và thông tin site sẽ không được gửi đến Microsoft. Tuy nhiên, nếu Microsoft Edge triển khai trên Windows 10 thì dữ liệu chẩn đoán và thông tin site sẽ được gửi theo thiết đặt dữ liệu [Windows chẩn đoán của người dùng.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Để cấu hình cách Microsoft Edge lý việc thu thập dữ liệu cho tổ chức của bạn, hãy dùng các chính sách nhóm sau đây:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Chính sách này cho phép báo cáo về mức sử dụng và dữ liệu liên quan đến sự cố.
- [SendSiteInfoToImproveServices:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices)Chính sách này gửi thông tin site được sử dụng để cải dịch vụ Microsoft.

Để tìm hiểu thêm, xem mục Đặt [cấu hình thiết đặt chính sách](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).