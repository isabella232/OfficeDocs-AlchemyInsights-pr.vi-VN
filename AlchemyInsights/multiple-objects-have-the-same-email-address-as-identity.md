---
title: Nhiều đối tượng có cùng địa chỉ email dưới dạng danh tính
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 5866d182cb2e97e37bc6df87e05fb6ef55bfed1d36f9daa95b7b8993a509e2dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011934"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Nhiều đối tượng có cùng địa chỉ email dưới dạng danh tính

**Nhiều đối tượng**

Một trong những lý do phổ biến của lỗi này là không thể định tuyến yêu cầu Outlook Web Access đúng cách trong trạng thái hiện diện của nhiều đối tượng có cùng địa chỉ email dưới dạng danh tính. Để tìm các đối tượng này, hãy chạy các lệnh sau đây:

· Get-Recipient <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact <email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

Để giải quyết sự cố này, hãy loại bỏ nhiều đối tượng có cùng một danh tính email và đảm bảo rằng có một đối tượng duy nhất có danh tính email cụ thể và loại người nhận là UserMailbox.

**Cùng một địa chỉ được dùng cho hộp thư doanh nghiệp và người tiêu dùng**

Một nguyên nhân khác là khi cùng một địa chỉ được dùng cho hộp thư doanh nghiệp và người tiêu dùng. Trong trường hợp này, người dùng phải thay đổi biệt danh người dùng chính của mình cho đến khi Cafe hỗ trợ kịch bản này. Đây là lỗi vĩnh viễn không biến mất mà không cần can thiệp.

Để biết chi tiết, hãy [xem Thay đổi địa chỉ email hoặc số điện thoại cho tài khoản Microsoft của bạn](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).