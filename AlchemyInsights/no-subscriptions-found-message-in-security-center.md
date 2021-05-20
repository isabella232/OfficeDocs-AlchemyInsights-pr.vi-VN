---
title: Thông báo Không tìm thấy đăng ký nào trong Trung tâm Bảo mật
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544130"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="812ca-102">Thông báo Không tìm thấy đăng ký nào trong Trung tâm Bảo mật</span><span class="sxs-lookup"><span data-stu-id="812ca-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="812ca-103">Nếu trong khi truy nhập Trung tâm Bảo mật của Bộ bảo vệ Microsoft bạn nhận được thông báo "Không tìm thấy đăng ký nào", nghĩa là Azure Active Directory (AAD) đã được sử dụng để đăng nhập người dùng vào cổng thông tin không có giấy phép ATP của Bộ bảo vệ Microsoft.</span><span class="sxs-lookup"><span data-stu-id="812ca-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="812ca-104">Giấy Windows E5 và Office E5 là các giấy phép riêng biệt.</span><span class="sxs-lookup"><span data-stu-id="812ca-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="812ca-105">Mở một trường hợp hỗ trợ nếu giấy phép đã được mua nhưng chưa được cung cấp cho phiên bản AAD này.</span><span class="sxs-lookup"><span data-stu-id="812ca-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="812ca-106">Bạn có thể:</span><span class="sxs-lookup"><span data-stu-id="812ca-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="812ca-107">Vấn đề cung cấp giấy phép có thể xảy ra.</span><span class="sxs-lookup"><span data-stu-id="812ca-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="812ca-108">Bạn vô tình cung cấp giấy phép cho một Microsoft AAD khác với giấy phép được dùng cho việc xác thực vào dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="812ca-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>