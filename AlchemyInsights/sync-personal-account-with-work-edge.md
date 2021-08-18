---
title: Cho phép người dùng đồng bộ tài khoản cá nhân với tài khoản cơ quan trong Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: ad4b64c4bb50f50d4ab9fa47bb37228dce538e6d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317300"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Cho phép người dùng đồng bộ tài khoản cá nhân với tài khoản cơ quan trong Microsoft Edge

Hãy đảm bảo bạn đáp ứng các tiêu chí này:

- Chuyển vùng Trạng thái Doanh nghiệp được bật trong trung tâm quản trị Azure Active Directory của Microsoft, trung tâm này yêu cầu phải có đăng ký để Azure Active Directory Premium hoặc Enterprise Mobility + Security (EMS). Để biết thêm thông tin, [hãy xem mục Bật Chuyển vùng Bang của Doanh nghiệp Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-enable)
- Một hoặc cả hai tiêu chí sau đây được đáp ứng:
    - Dịch vụ Azure Information Protection được kích hoạt cho đối tượng thuê của bạn. Để biết chi tiết, [hãy xem mục Kích hoạt bảo vệ Azure Rights Management từ Trung tâm quản trị Microsoft 365.](https://docs.microsoft.com/azure/information-protection/activate-office365)
    - Tính năng Azure Active Directory Chuyển vùng Bang Doanh nghiệp (ESR) được bật cho bất kỳ người dùng hoặc đối tượng thuê nào. Để biết thêm thông tin, hãy [xem Chuyển vùng trạng thái doanh nghiệp là gì?](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-overview).

Nếu AIP và ESR đều bị vô hiệu hóa, một thông báo lỗi sẽ thông báo cho người dùng rằng đồng bộ không sẵn dùng cho tài khoản của họ.
