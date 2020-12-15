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
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge đặt cấu hình thiết đặt quyền riêng tư

Theo mặc định, nếu Microsoft Edge được triển khai trên nền tảng không phải Windows, dữ liệu chẩn đoán và thông tin site sẽ không được gửi đến Microsoft. Tuy nhiên, nếu Microsoft Edge được triển khai trên Windows 10, dữ liệu chẩn đoán và thông tin site được gửi theo [cài đặt dữ liệu chẩn đoán Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)của người dùng.

Để cấu hình cách Microsoft Edge xử lý thu thập dữ liệu cho tổ chức của bạn, hãy sử dụng các chính sách nhóm sau đây:
- [Metricsreportingenabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): chính sách này cho phép báo cáo về việc sử dụng và dữ liệu liên quan đến sự cố.
- [Sendsiteinfotoimproveservices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): chính sách này sẽ gửi thông tin site được dùng để cải thiện các dịch vụ của Microsoft.

Để tìm hiểu thêm, hãy xem [cấu hình thiết đặt chính sách](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).