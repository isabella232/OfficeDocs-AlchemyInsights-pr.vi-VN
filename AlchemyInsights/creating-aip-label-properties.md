---
title: Tạo chính sách nhãn AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732197"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="4c760-102">Tạo chính sách nhãn AIP</span><span class="sxs-lookup"><span data-stu-id="4c760-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="4c760-103">Nhãn bảo vệ thông tin Azure (AIP) có thể được sử dụng với đầy đủ các dữ liệu mà một tổ chức thường tạo và lưu trữ, từ phân loại dữ liệu cá nhân thấp nhất, đến phân loại cao nhất của dữ liệu bảo mật cao.</span><span class="sxs-lookup"><span data-stu-id="4c760-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="4c760-104">Các chính sách bảo vệ thông tin Azure áp dụng cho máy khách cổ điển thông tin Azure (AIP) và không phải máy  [khách gắn nhãn hợp nhất của AIP](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="4c760-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="4c760-105">Bạn có thể cấu hình nhiều thành phần trong chính sách AIP, bao gồm các tùy chọn như sau:</span><span class="sxs-lookup"><span data-stu-id="4c760-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="4c760-106">Tùy chọn mà nhãn nào sẽ cho phép người quản trị hoặc các tài liệu phân loại và bảo vệ của người dùng (tùy chọn) và email</span><span class="sxs-lookup"><span data-stu-id="4c760-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="4c760-107">Tùy chọn để thực thi phân loại khi người dùng lưu tài liệu và gửi email</span><span class="sxs-lookup"><span data-stu-id="4c760-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="4c760-108">Tùy chọn tự động gắn nhãn thông điệp email, dựa vào tệp đính kèm của nó.</span><span class="sxs-lookup"><span data-stu-id="4c760-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="4c760-109">Tùy chọn để kiểm soát xem thanh bảo vệ thông tin có được hiển thị trong các ứng dụng Office hay không</span><span class="sxs-lookup"><span data-stu-id="4c760-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="4c760-110">Để biết các tùy chọn và thông tin bổ sung về các chính sách bảo vệ thông tin Azure, hãy xem: [tổng quan về chính sách bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="4c760-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="4c760-111">Để biết các tài nguyên hữu ích khác về chính sách AIP, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="4c760-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="4c760-112">Hướng dẫn: đặt cấu hình thiết đặt chính sách bảo vệ thông tin Azure và tạo nhãn mới</span><span class="sxs-lookup"><span data-stu-id="4c760-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="4c760-113">Cấu hình chính sách bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="4c760-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="4c760-114">Tạo và cấu hình nhãn nhạy cảm và chính sách của họ</span><span class="sxs-lookup"><span data-stu-id="4c760-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="4c760-115">Hướng dẫn cách làm cho các tình huống thông thường sử dụng bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="4c760-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="4c760-116">Xem lại tài liệu bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="4c760-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="4c760-117">Các yêu cầu về bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="4c760-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="4c760-118">Hướng dẫn nhanh về bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="4c760-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="4c760-119">Tải xuống máy khách bảo vệ thông tin về Azure</span><span class="sxs-lookup"><span data-stu-id="4c760-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)