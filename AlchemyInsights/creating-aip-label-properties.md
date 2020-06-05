---
title: Създаване на правила за AIP етикет
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/03/2020
ms.locfileid: "44568916"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="b8b25-102">Създаване на правила за AIP етикет</span><span class="sxs-lookup"><span data-stu-id="b8b25-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="b8b25-103">Етикетите за защита на информацията в Azure (AIP) могат да се използват с пълния набор от данни, които организацията обикновено създава и съхранява от най-ниската класификация на личните данни до най-високата класификация на силно поверителни данни.</span><span class="sxs-lookup"><span data-stu-id="b8b25-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="b8b25-104">Правилата за защита на информацията в Azure се прилагат към класическия клиент за защита на информацията (AIP) на Azure, а не [към AIP unified Labeling клиента.](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)</span><span class="sxs-lookup"><span data-stu-id="b8b25-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="b8b25-105">Можете да конфигурирате няколко елемента в правила за ЕНП, включително опции като:</span><span class="sxs-lookup"><span data-stu-id="b8b25-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="b8b25-106">Опция, за която ще позволи на администраторите или потребителя да класифицират и защитават (по избор) документи и имейли</span><span class="sxs-lookup"><span data-stu-id="b8b25-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="b8b25-107">Възможност за прилагане на класификация, когато потребителите записват документи и изпращане на имейл</span><span class="sxs-lookup"><span data-stu-id="b8b25-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="b8b25-108">Опция за автоматично маркиране на имейл съобщение въз основа на прикачените файлове.</span><span class="sxs-lookup"><span data-stu-id="b8b25-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="b8b25-109">Възможност за контрол дали лента за защита на информацията се показва в приложения на Office</span><span class="sxs-lookup"><span data-stu-id="b8b25-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="b8b25-110">За допълнителни опции и информация относно правилата за защита на информацията в Azure вижте: [Преглед на правилата за защита на информацията на Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="b8b25-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="b8b25-111">За други полезни ресурси относно правилата за AIP вижте:</span><span class="sxs-lookup"><span data-stu-id="b8b25-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="b8b25-112">Въвеждащ курс: Конфигуриране на настройките за правилата за защита на информацията в Azure и създаване на нов етикет</span><span class="sxs-lookup"><span data-stu-id="b8b25-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="b8b25-113">Конфигуриране на правилата за защита на информацията в Azure</span><span class="sxs-lookup"><span data-stu-id="b8b25-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="b8b25-114">Създаване и конфигуриране на етикети за чувствителност и техните правила</span><span class="sxs-lookup"><span data-stu-id="b8b25-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="b8b25-115">Как да се водят за често срещани сценарии, които използват azure информация за защита</span><span class="sxs-lookup"><span data-stu-id="b8b25-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="b8b25-116">Преглед на документацията за защита на информацията в Azure</span><span class="sxs-lookup"><span data-stu-id="b8b25-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="b8b25-117">Изисквания за защита на информацията в Azure</span><span class="sxs-lookup"><span data-stu-id="b8b25-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="b8b25-118">Ръководство за бърз старт за защита на информацията в Azure</span><span class="sxs-lookup"><span data-stu-id="b8b25-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="b8b25-119">Изтегляне на клиент за защита на информацията в Azure</span><span class="sxs-lookup"><span data-stu-id="b8b25-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)