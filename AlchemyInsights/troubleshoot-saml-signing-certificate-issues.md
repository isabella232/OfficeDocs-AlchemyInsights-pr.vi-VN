---
title: Khắc phục sự cố chứng chỉ ký vào SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694455"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="880d2-102">Khắc phục sự cố chứng chỉ ký vào SAML</span><span class="sxs-lookup"><span data-stu-id="880d2-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="880d2-103">Để giải quyết sự cố về chứng chỉ ký hợp nhất, hãy thực hiện các bước được đề xuất sau đây:</span><span class="sxs-lookup"><span data-stu-id="880d2-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="880d2-104">Khi bạn thêm ứng dụng doanh nghiệp hỗ trợ SSO, Azure sẽ tạo ra một chứng chỉ được gọi là [chứng chỉ ký SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="880d2-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="880d2-105">Chứng chỉ này có ngày hết hạn 3 năm.</span><span class="sxs-lookup"><span data-stu-id="880d2-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="880d2-106">Để thay đổi ngày hết hạn chứng chỉ của bạn, hãy xem [tùy chỉnh ngày hết hạn cho chứng chỉ liên kết của bạn và cuộn nó sang chứng chỉ mới](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="880d2-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="880d2-107">Azure sẽ dùng chứng chỉ này để ký thẻ SAML được yêu cầu bởi ứng dụng và gửi qua ứng dụng cho một SSO thành công.</span><span class="sxs-lookup"><span data-stu-id="880d2-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="880d2-108">Để hoàn tất việc này, hãy tải xuống chứng chỉ từ cổng thông tin Azure và gửi nó đến nhà cung cấp ứng dụng để hoàn tất quy trình SSO.</span><span class="sxs-lookup"><span data-stu-id="880d2-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="880d2-109">Sau khi quá trình này hoàn thành ứng dụng của bạn sẽ tin cậy chứng chỉ này và tất cả các thẻ SAML được ký bằng chứng chỉ này sẽ được ứng dụng chấp nhận.</span><span class="sxs-lookup"><span data-stu-id="880d2-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="880d2-110">Nếu chứng chỉ này hết hạn, hãy tạo chứng chỉ mới, Cập Nhật tài liệu đó vào nhà cung cấp ứng dụng, rồi làm cho nó hiện hoạt trên Azure bên.</span><span class="sxs-lookup"><span data-stu-id="880d2-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="880d2-111">Để biết thêm thông tin, hãy xem gia [hạn một chứng chỉ sẽ sớm hết hạn](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="880d2-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="880d2-112">Nếu chứng chỉ hết hạn, thì người dùng sẽ không bị chặn.</span><span class="sxs-lookup"><span data-stu-id="880d2-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="880d2-113">[Thêm một địa chỉ email để nhận thông báo](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) sẽ được nhận trước khi chứng chỉ hiện tại hết hạn.</span><span class="sxs-lookup"><span data-stu-id="880d2-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="880d2-114">Bước-4 là một tùy chọn.</span><span class="sxs-lookup"><span data-stu-id="880d2-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="880d2-115">Thay đổi tùy chọn ký chứng chỉ SAML của ứng dụng và thuật toán ký chứng chỉ.</span><span class="sxs-lookup"><span data-stu-id="880d2-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="880d2-116">Để biết thêm thông tin, hãy xem mục [thay đổi tùy chọn ký chứng chỉ và thuật toán ký](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="880d2-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

