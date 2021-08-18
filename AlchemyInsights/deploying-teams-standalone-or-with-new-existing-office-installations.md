---
title: Triển khai Teams ở dạng độc lập hoặc với các bản cài đặt Office mới hoặc hiện có
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320144"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Triển khai Teams ở dạng độc lập hoặc với các bản cài đặt Office mới hoặc hiện có

Microsoft Teams này hiện đã được  tích hợp như một phần trong các bản cài đặt mới của Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn, Ứng dụng Microsoft 365 dành cho doanh nghiệp và Office for Mac. Để biết thêm thông tin, [hãy xem mục Khi nào Microsoft Teams đầu được tích hợp với các bản cài đặt mới của Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Ngoài ra, bắt đầu với Phiên bản 1906  trong Kênh Hiện tại, Teams sẽ được thêm vào các bản cài đặt hiện có của Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn (và Ứng dụng Microsoft 365 dành cho doanh nghiệp) trên các thiết bị chạy Windows khi bạn cập nhật bản cài đặt hiện có của mình lên phiên bản mới nhất. Để biết thêm thông tin, [hãy xem mục Thông tin về các bản cài đặt hiện có của Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Lưu** ý : Nếu bạn không muốn chờ lịch trình triển khai này, bạn có [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) thể triển khai Teams dưới dạng độc lập cho người dùng của mình bằng cách làm theo các hướng dẫn sau hoặc bạn có thể yêu cầu người dùng cài đặt Teams cho chính mình từ [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Nếu tổ chức của bạn chưa sẵn sàng triển khai Teams, chúng tôi có [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) các [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) bước bạn có thể thực hiện để loại trừ ***Teams*** khỏi các bản cài đặt mới hoặc hiện Office. Nếu bạn muốn cài Teams nhưng không muốn Teams bắt đầu tự động cho người dùng sau khi đã cài đặt ứng dụng, hãy xem mục Ngăn không cho Microsoft Teams khởi động tự động sau khi cài [đặt.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Để ***gỡ cài Teams cài*** đặt khỏi thiết bị đang chạy Windows, hãy xem gỡ cài đặt [Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Để dọn dẹp Microsoft Teams người dùng hoặc máy đích, hãy xem mục dọn [Microsoft Teams khai mới.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Nếu bạn đang sử dụng máy tính dùng chung, Dịch vụ Máy tính Từ xa (RDS) hoặc Cơ sở hạ tầng Máy tính Ảo (VDI), hãy xem Máy tính dùng chung và môi trường [VDI với các Microsoft Teams.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

Nếu bạn đang sử dụng Office for Mac, xem mục Cài [Microsoft Teams đặt trên máy Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**Lưu** ý : Sau khi Teams được cài đặt, nó sẽ tự động cập nhật [khoảng](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) hai tuần một lần với các tính năng mới và cập nhật chất lượng. 