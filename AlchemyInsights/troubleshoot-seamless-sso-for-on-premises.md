---
title: Khắc phục sự cố đăng nhập đơn (SSO) tại cơ sở
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816344"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="960c5-102">Khắc phục sự cố đăng nhập đơn (SSO) tại cơ sở</span><span class="sxs-lookup"><span data-stu-id="960c5-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="960c5-103">Để giải quyết các sự cố đăng nhập đơn (SSO), hãy thực hiện các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="960c5-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="960c5-104">**Làm thế nào tôi có thể cuộn qua khóa giải mã Kerberos của tài khoản máy tính AZUREADSSO?**</span><span class="sxs-lookup"><span data-stu-id="960c5-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="960c5-105">Chúng tôi khuyên bạn nên cuộn qua khóa giải mã Kerberos trong ít nhất mỗi 30 ngày.</span><span class="sxs-lookup"><span data-stu-id="960c5-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="960c5-106">Để thực hiện điều này theo cách thủ công, hãy xem [làm thế nào để cuộn qua các khóa giải mã Kerberos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span><span class="sxs-lookup"><span data-stu-id="960c5-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="960c5-107">**Cấu hình SSO liền mạch**</span><span class="sxs-lookup"><span data-stu-id="960c5-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="960c5-108">Để triển khai SSO liền mạch, hãy làm theo các bước trong [Azure Active Directory seamless đăng nhập đơn: bắt đầu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys)nhanh.</span><span class="sxs-lookup"><span data-stu-id="960c5-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="960c5-109">**Cố**</span><span class="sxs-lookup"><span data-stu-id="960c5-109">**Advisory**</span></span>

- <span data-ttu-id="960c5-110">[Azure Active Directory seamless Single Sign-on: câu hỏi thường gặp](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) -trong bài viết này, chúng tôi địa chỉ câu hỏi thường gặp về Azure Active Directory seamless Sign-On đơn (SSO liền mạch).</span><span class="sxs-lookup"><span data-stu-id="960c5-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="960c5-111">Hãy kiểm tra lại nội dung mới.</span><span class="sxs-lookup"><span data-stu-id="960c5-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="960c5-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) -bài viết này cung cấp thông tin về cách thực hiện các yêu cầu về tính năng hoặc đặt câu hỏi kỹ thuật về SSO liền mạch.</span><span class="sxs-lookup"><span data-stu-id="960c5-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="960c5-113">**Đoán**</span><span class="sxs-lookup"><span data-stu-id="960c5-113">**Troubleshoot**</span></span>

<span data-ttu-id="960c5-114">[Khắc phục sự cố Azure Active Directory liền mạch Single đăng nhập](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) -bài viết này sẽ giúp bạn tìm thấy thông tin khắc phục sự cố về các vấn đề thường gặp về Azure Active Directory (Azure AD) Sign-On đơn nhất (SSO liền mạch).</span><span class="sxs-lookup"><span data-stu-id="960c5-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







