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
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813411"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Cho phép người dùng đồng bộ tài khoản cá nhân với tài khoản cơ quan trong Microsoft Edge

Hãy đảm bảo bạn đáp ứng các tiêu chí này:

- Chuyển vùng Trạng thái Doanh nghiệp được bật trong trung tâm quản trị Azure Active Directory của Microsoft, trung tâm này yêu cầu phải có đăng ký để Azure Active Directory Premium hoặc Enterprise Mobility + Security (EMS). Để biết thêm thông tin, [hãy xem mục Bật Chuyển vùng Bang doanh nghiệp Azure Active Directory.](/azure/active-directory/devices/enterprise-state-roaming-enable)
- Một hoặc cả hai tiêu chí sau đây được đáp ứng:
    - Dịch vụ Azure Information Protection được kích hoạt cho đối tượng thuê của bạn. Để biết chi tiết, [hãy xem mục Kích hoạt bảo vệ Azure Rights Management từ Trung tâm quản trị Microsoft 365.](/azure/information-protection/activate-office365)
    - Tính Azure Active Directory Chuyển vùng Bang Enterprise (ESR) được bật cho bất kỳ người dùng hoặc đối tượng thuê nào. Để biết thêm thông tin, hãy [xem Chuyển vùng trạng thái doanh nghiệp là gì?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Nếu AIP và ESR đều bị vô hiệu hóa, một thông báo lỗi sẽ thông báo cho người dùng rằng đồng bộ không sẵn dùng cho tài khoản của họ.
