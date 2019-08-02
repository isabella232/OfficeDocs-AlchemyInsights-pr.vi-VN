---
title: Triển khai các đội như độc lập hoặc với bản cài đặt mới hoặc hiện tại văn phòng
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054252"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Triển khai các đội như độc lập hoặc với bản cài đặt mới hoặc hiện tại văn phòng

Microsoft Teams bây giờ là bao gồm như là một phần của ***bản cài đặt mới*** của Office 365 ProPlus, Office 365 doanh nghiệp và văn phòng cho Mac. Để biết thêm thông tin, hãy xem [khi sẽ Microsoft Teams bắt đầu được bao gồm trong các cài đặt mới của Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Ngoài ra, bắt đầu với phiên bản năm 1906 trong kênh hàng tháng, các đội sẽ là ***Thêm vào hiện tại cơ sở*** của Office 365 ProPlus (và Office 365 doanh nghiệp) trên thiết bị chạy Windows khi bạn cập nhật cài đặt hiện có của bạn lên phiên bản mới nhất. Để biết thêm thông tin, hãy xem [những gì về các cài đặt hiện có của văn phòng?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Nếu bạn không muốn chờ đợi cho lịch trình buổi giới thiệu này, bạn có thể triển khai các đội như độc lập cho người dùng của bạn bằng cách làm [theo các hướng dẫn sau](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) hoặc bạn có thể có người dùng cài đặt các đội cho mình từ [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Nếu tổ chức của bạn không sẵn sàng để triển khai các đội, chúng tôi có các bước bạn có thể để ***loại trừ các đội*** từ cài đặt [mới](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) hoặc [hiện tại](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) của văn phòng. Nếu bạn muốn các đội được cài đặt, nhưng không muốn đội để tự khởi động cho người dùng sau khi nó được cài đặt, xem [Ngăn chặn Microsoft đội từ bắt đầu tự động sau khi cài đặt](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Để ***gỡ bỏ cài đặt các đội*** từ một thiết bị chạy Windows, hãy xem [Uninstall Microsoft đội](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Để dọn dẹp Microsoft Teams nhiều mục tiêu máy hoặc người dùng, hãy xem [triển khai Microsoft đội dọn dẹp](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Nếu bạn đang sử dụng máy tính được chia sẻ, Dịch vụ máy tính để bàn từ xa (RDS) hoặc máy tính để bàn ảo cơ sở hạ tầng (VDI), xem các [máy tính được chia sẻ và VDI môi trường với Microsoft đội](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Nếu bạn đang sử dụng Office cho Mac, hãy xem [Microsoft đội cài đặt trên máy Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Sau khi các đội được cài đặt, nó là [tự động Cập Nhật](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) khoảng mỗi hai tuần với các tính năng mới và Cập Nhật chất lượng. 