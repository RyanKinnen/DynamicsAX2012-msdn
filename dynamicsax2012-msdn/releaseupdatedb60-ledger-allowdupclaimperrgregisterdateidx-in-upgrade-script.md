﻿---
title: ReleaseUpdateDB60_Ledger.allowDupClaimPerRGRegisterDateIdx_IN Upgrade Script
TOCTitle: ReleaseUpdateDB60_Ledger.allowDupClaimPerRGRegisterDateIdx_IN Upgrade Script
ms:assetid: 841709cf-d5e1-764c-638f-bdf3f1285a1c
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ685997(v=AX.60)
ms:contentKeyID: 49709450
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateDB60\_Ledger.allowDupClaimPerRGRegisterDateIdx\_IN Upgrade Script 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2, Microsoft Dynamics AX 2012 Feature Pack, Microsoft Dynamics AX 2012_

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Class</strong></p></td>
<td><p>ReleaseUpdateDB60_Ledger</p></td>
</tr>
<tr class="even">
<td><p><strong>Method</strong></p></td>
<td><p>allowDupClaimPerRGRegisterDateIdx_IN</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Updates the RGRegisterDateIdx index in the ClaimPercentage_IN table to allow for duplicate records.</p></td>
</tr>
</tbody>
</table>


## Affected Modules and Tables

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Affected Modules</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Ledger</p></td>
</tr>
</tbody>
</table>


<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Affected Tables</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>ClaimPercentage_IN</p></td>
</tr>
</tbody>
</table>


## Remarks

The TaxComponent field is replaced with the new TaxComponentTable surrogate key field in the RGRegisterDateIdx unique index. Also, the FromDate and ToDate fields are replaced with the DateEffectivity, ValidFrom and ValidTo fields. Initially these fields contain no values. So the index is set to allow for duplicates before the field is updated with the value of the record IDs of the corresponding tables.

  


