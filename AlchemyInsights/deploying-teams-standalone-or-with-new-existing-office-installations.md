---
title: Triển khai teams là độc lập hoặc với cài đặt Office mới hoặc hiện tại
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 4b843407f05db207f3b676c03c7088d3d0ba062e
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704655"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Triển khai teams là độc lập hoặc với cài đặt Office mới hoặc hiện tại

Microsoft teams hiện đã được đưa vào như một phần của các ***cài đặt mới*** của Microsoft 365 ứng dụng dành cho doanh nghiệp, Microsoft 365 ứng dụng dành cho doanh nghiệp và Office cho Mac. Để biết thêm thông tin, xem [khi nào Microsoft teams sẽ bắt đầu được đưa vào cài đặt Office mới?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Ngoài ra, bắt đầu với phiên bản 1906 trong hàng tháng kênh, nhóm sẽ được ***Thêm vào cài đặt hiện*** tại của Microsoft 365 ứng dụng dành cho doanh nghiệp (và Microsoft 365 ứng dụng dành cho doanh nghiệp) trên thiết bị chạy Windows khi bạn cập nhật cài đặt hiện có phiên bản mới nhất. Để biết thêm thông tin, xem [những gì về cài đặt hiện tại của Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Nếu bạn không muốn chờ đợi lịch trình triển khai này, bạn có thể sử dụng teams là độc lập cho người dùng bằng cách  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)làm [theo các hướng dẫn này](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)hoặc bạn có thể tự cài đặt nhóm của mình.

Nếu tổ chức của bạn chưa sẵn sàng triển khai teams, chúng tôi có các bước bạn có thể thực hiện để ***loại trừ teams*** khỏi cài đặt Office [mới](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) hoặc [hiện tại](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) . Nếu bạn muốn cài đặt teams, nhưng không muốn teams tự động bắt đầu cho người dùng sau khi cài đặt, hãy xem [ngăn Microsoft teams tự động bắt đầu sau khi cài đặt](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Để ***gỡ cài đặt teams*** khỏi thiết bị chạy Windows, xem [dỡ cài đặt Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Để dọn dẹp Microsoft teams từ nhiều máy mục tiêu hoặc người dùng, xem [triển khai Microsoft teams dọn sạch](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Nếu bạn đang sử dụng máy tính dùng chung, Dịch vụ máy tính để bàn từ xa (RDS) hoặc cơ sở hạ tầng máy tính ảo (VDI), hãy xem [máy tính dùng chung và môi trường VDI với Microsoft teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Nếu bạn đang sử dụng Office cho Mac, hãy xem [cài đặt Microsoft teams trên máy Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Sau khi teams được cài đặt, nó [tự động Cập Nhật](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) khoảng mỗi hai tuần với các tính năng và Cập Nhật chất lượng mới. 