---
title: Cách bật thư thoại được lưu trữ
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679160"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="d34c6-102">Cách bật thư thoại được lưu trữ</span><span class="sxs-lookup"><span data-stu-id="d34c6-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="d34c6-103">Để bật thư thoại, **Hosteivoicemail** phải được đặt là $true.</span><span class="sxs-lookup"><span data-stu-id="d34c6-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="d34c6-104">Thuộc tính **Hostedvoicemail** trên người dùng bằng cách sử dụng Remote PowerShell (RPS).</span><span class="sxs-lookup"><span data-stu-id="d34c6-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="d34c6-105">Để biết thêm thông tin về kết nối đến RPS, hãy xem [tổng quan về Microsoft nhóm PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) để biết thêm thông tin về kết nối đến RPS.</span><span class="sxs-lookup"><span data-stu-id="d34c6-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="d34c6-106">Người quản trị nhóm phải được đăng nhập vào PowerShell từ xa cho các nhóm.</span><span class="sxs-lookup"><span data-stu-id="d34c6-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="d34c6-107">Từ PowerShell nhắc người quản trị nhóm có thể chạy **Set-csuser user@contoso.com-hostetin thư thoại $True** nơi mà URI SIP là người dùng trong câu hỏi.</span><span class="sxs-lookup"><span data-stu-id="d34c6-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="d34c6-108">Những thay đổi đối với các chính sách có thể mất tối đa 24 giờ để sao chép.</span><span class="sxs-lookup"><span data-stu-id="d34c6-108">Changes to policies can take up to 24 hours to replicate.</span></span>