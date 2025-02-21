---
title: DeviceTvmSecureConfigurationAssessmentKB table in the Advanced hunting schema
description: Learn about the various secure configurations assessed by Threat & Vulnerability Management in the DeviceTvmSecureConfigurationAssessmentKB table of the Advanced hunting schema. 
keywords: advanced hunting, threat hunting, cyber threat hunting, search, query, telemetry, schema reference, kusto, table, column, data type, description, threat & vulnerability management, TVM, device management, security configuration, MITRE ATT&CK framework, knowledge base, KB, DeviceTvmSecureConfigurationAssessmentKB
search.product: eADQiWindows 10XVcnh
search.appverid: met150
ms.prod: w10
ms.mktglfcycl: deploy
ms.sitesec: library
ms.pagetype: security
ms.author: dolmont
author: DulceMontemayor
ms.localizationpriority: medium
manager: dansimp
audience: ITPro
ms.collection: M365-security-compliance 
ms.topic: article
ms.date: 11/12/2019
---

# DeviceTvmSecureConfigurationAssessmentKB

**Applies to:**

- [Microsoft Defender Advanced Threat Protection (Microsoft Defender ATP)](https://go.microsoft.com/fwlink/p/?linkid=2069559)

>Want to experience Microsoft Defender ATP? [Sign up for a free trial.](https://www.microsoft.com/en-us/WindowsForBusiness/windows-atp?ocid=docs-wdatp-advancedhuntingref-abovefoldlink)

[!include[Prerelease information](prerelease.md)]

The DeviceTvmSecureConfigurationAssessmentKB table in the Advanced hunting schema contains information about the various secure configurations — such as whether a device has automatic updates on — checked by [Threat & Vulnerability Management](next-gen-threat-and-vuln-mgt.md). It also includes risk information, related industry benchmarks, and applicable MITRE ATT&CK techniques and tactics. Use this reference to construct queries that return information from the table.

For information on other tables in the Advanced hunting schema, see [the Advanced hunting reference](advanced-hunting-reference.md).

| Column name | Data type | Description |
|-------------|-----------|-------------|
| ConfigurationId | string | Unique identifier for a specific configuration |
| ConfigurationImpact | string | Rated impact of the configuration to the overall configuration score (1-10) |
| ConfigurationName | string | Display name of the configuration |
| ConfigurationDescription | string | Description of the configuration |
| RiskDescription | string | Description of the associated risk |
| ConfigurationCategory | string | Category or grouping to which the configuration belongs: Application, OS, Network, Accounts, Security controls|
| ConfigurationSubcategory | string |Subcategory or subgrouping to which the configuration belongs. In many cases, this describes specific capabilities or features. |
| ConfigurationBenchmarks | string | List of industry benchmarks recommending the same or similar configuration |
| RelatedMitreTechniques | string | List of Mitre ATT&CK framework techniques related to the configuration |
| RelatedMitreTactics  | string | List of Mitre ATT&CK framework tactics related to the configuration |

## Related topics

- [Advanced hunting overview](overview-hunting.md)
- [All Advanced hunting tables](advanced-hunting-reference.md)
- [Advanced hunting query best practices](advanced-hunting-best-practices.md)
- [Query data using Advanced hunting](advanced-hunting.md)
- [Overview of Threat & Vulnerability Management](next-gen-threat-and-vuln-mgt.md)
