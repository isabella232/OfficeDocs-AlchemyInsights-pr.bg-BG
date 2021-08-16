---
title: Intune Exchange on-premise Connector
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013953"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange on-premise Connector

За подробности относно настройването на конектора между Intune и Exchange, който се хоства локално, вижте следната документация:

[Настройване на локалния конектор на Intune Exchange в Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**ЧЗВ:**

В: Виждам грешка, като например "Версията Exchange Connector не се поддържа", когато се опитвате да настроите Exchange конектора. Каква може да е причината?

О: Акаунтът, който използвате, е лицензиран по подходящ начин – той трябва да има активен лиценз за Intune

В: Възможно ли е да имате няколко Exchange конектора?

A: Можете да настроите само един Exchange за клиент на Intune за Exchange организация. Конекторът може да се инсталира само на един сървър в организация за обмен на много сървъри.

Също така не можете да конфигурирате конектори както за Exchange на място, така и за Exchange Online конфигурирани в един и същ клиент.

В: Може ли конекторът да използва CAS масив като връзка към Exchange?

О: Задаването на CAS масив не е поддържана конфигурация в настройката на конектора. Трябва да бъде зададен само един сървър и трябва да бъде кодиран в конфигурационния файл на конектора, който може да се намери в

програмни данни\microsoft\microsoft Intune на предварително Exchange конектор\ OnpremiseExchangeConnectorServiceConfiguration.xml

Намерете следния запис и ```<ExchangeWebServiceURL />``` заместете URL адреса със сървъра за exchange.

**Пример:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Вижте следната документация за допълнителни отстраняване на [неизправности: Отстраняване на неизправности в локалния Exchange Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Разрешаване на многослойното регистриране за Exchange конектор**

1. Отворете конфигурационния Exchange за проследяване на конектора за редактиране.  
Файлът се намира на: %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Пример:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Намерете TraceSourceLine със следния ключ: OnPremisesExchangeConnectorService  
  
3. Промяна на стойността на възела SourceLevel от Информационна дейностТракиране (по подразбиране) на Verbose ActivityTracing  

**Пример:**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Рестартиране на Microsoft Intune Exchange услугата  
5. Пълно синхронизиране в портала на Intune, докато не завърши, и след това променете XML отново на "Информационна дейностПроследяване" и рестартирайте Microsoft Intune Exchange услугата.  
6. Местоположението на регистрационните файлове е: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`