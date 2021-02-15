---
title: Парола нефиксирани не работи
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243231"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="ee100-102">Парола нефиксирани не работи</span><span class="sxs-lookup"><span data-stu-id="ee100-102">Password Writeback is not working</span></span>

<span data-ttu-id="ee100-103">**Имам проблеми с конфигурирането на парола нефиксирани**</span><span class="sxs-lookup"><span data-stu-id="ee100-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="ee100-104">Password нефиксирани е функция Premium.</span><span class="sxs-lookup"><span data-stu-id="ee100-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="ee100-105">Уверете се, че разбирате изискванията за лицензиране:</span><span class="sxs-lookup"><span data-stu-id="ee100-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="ee100-106">Трябва да имате поне един лиценз, присвоен във вашата организация</span><span class="sxs-lookup"><span data-stu-id="ee100-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="ee100-107">**Потребители в облака** – всеки Office 365 (O365) платен SKU или Azure ad Basic</span><span class="sxs-lookup"><span data-stu-id="ee100-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="ee100-108">**Облак и/или локални потребители** – Azure ad Premium P1 или P2, корпоративна мобилност + защита (EMS) или защитено продуктивно предприятие (спе)</span><span class="sxs-lookup"><span data-stu-id="ee100-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="ee100-109">За да научите повече за изискванията за лицензиране, вижте [лицензионни изисквания за услугата за самостоятелно нулиране на пароли на AZURE ad](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="ee100-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="ee100-110">Имате поне един акаунт на администратор и един тестов потребителски акаунт с един от подходящите лицензи.</span><span class="sxs-lookup"><span data-stu-id="ee100-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="ee100-111">Трябва да свържете Azure AD Connect към основния емулатор на домейнов контролер за работа с нефиксирани за парола.</span><span class="sxs-lookup"><span data-stu-id="ee100-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="ee100-112">Можете да конфигурирате Azure AD Connect, за да използвате първичен домейнов контролер, като щракнете с десния бутон върху **свойствата** на конектора за синхронизация на Active Directory и след това изберете **Конфигуриране на дялове на директорията**.</span><span class="sxs-lookup"><span data-stu-id="ee100-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="ee100-113">От там потърсете секцията **Настройки на връзката с домейновия контролер** и поставете отметка в квадратчето титулувани **Използвайте само предпочитани домейнови контролери**.</span><span class="sxs-lookup"><span data-stu-id="ee100-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="ee100-114">Ако предпочитан DC не е PDC емулатор, Azure AD Connect все още ще достигне до PDC за парола нефиксирани.</span><span class="sxs-lookup"><span data-stu-id="ee100-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="ee100-115">Нулирането на паролата е конфигурирано и разрешена във вашия клиент.</span><span class="sxs-lookup"><span data-stu-id="ee100-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="ee100-116">За повече информация вижте [Разрешаване на потребителите да нулират своите пароли за AZURE ad](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span><span class="sxs-lookup"><span data-stu-id="ee100-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="ee100-117">Уверете се, че акаунтът на администратора, който се използва за разрешаване на Password нефиксирани, е акаунт за администратора на облака (създаден в Azure AD not локален AD)</span><span class="sxs-lookup"><span data-stu-id="ee100-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="ee100-118">Разполагате с една или много горска РЕКЛАМНА локална инсталация с Windows Server 2008 R2, Windows Server 2012 или Windows Server 2012 R2 с инсталирани най-новите сервизни пакети</span><span class="sxs-lookup"><span data-stu-id="ee100-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="ee100-119">Разполагате с инсталиран инструмент за свързване на Azure AD и сте подготвили вашата РЕКЛАМНА среда за синхронизация на облака.</span><span class="sxs-lookup"><span data-stu-id="ee100-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="ee100-120">Преди да изпробвате Password нефиксирани, се уверете, че за първи път сте завършили пълно импортиране и пълно синхронизиране от AD и Azure AD в Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="ee100-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="ee100-121">За да научите повече, вижте как да направите [пълно синхронизиране и да импортирате изцяло в AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="ee100-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="ee100-122">**Имам проблем със свързването с парола нефиксирани**</span><span class="sxs-lookup"><span data-stu-id="ee100-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="ee100-123">Изтегляне и разрешаване на най-новата версия на [AZURE ad Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="ee100-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="ee100-124">Конфигурация на защитната стена: Инструментът за свързване на Azure AD (1.1.443 и по-нови версии) ще трябва да има **ИЗХОДЯЩ HTTPS** достъп до:</span><span class="sxs-lookup"><span data-stu-id="ee100-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="ee100-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ee100-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="ee100-126">servicebus. Windows. Networks</span><span class="sxs-lookup"><span data-stu-id="ee100-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="ee100-127">Позволяване на неактивни връзки да се запазят най-малко за 2-3 минути</span><span class="sxs-lookup"><span data-stu-id="ee100-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="ee100-128">**Все още имам проблеми с паролата нефиксирани**</span><span class="sxs-lookup"><span data-stu-id="ee100-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="ee100-129">Ако все още имате проблеми, опитайте да забраните и да активирате повторно услугата за нефиксирани на парола в инструмента за свързване на Azure AD</span><span class="sxs-lookup"><span data-stu-id="ee100-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="ee100-130">За да научите повече, вижте как да [забраните и активирате повторно парола нефиксирани](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="ee100-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
