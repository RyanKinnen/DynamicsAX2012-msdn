﻿---
title: ReleaseUpdateDB60_Ledger.allowNoDupDimensionAttributeSetHashIdx Upgrade Script
TOCTitle: ReleaseUpdateDB60_Ledger.allowNoDupDimensionAttributeSetHashIdx Upgrade Script
ms:assetid: 5bd89e71-1504-0401-df00-deacb9a0c631
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ736317(v=AX.60)
ms:contentKeyID: 49708492
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateDB60\_Ledger.allowNoDupDimensionAttributeSetHashIdx Upgrade Script 


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
<td><p>allowNoDupDimensionAttributeSetHashIdx</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Updates the HashIdx index in the DimensionAttributeSet table not to allow for duplicate records.</p></td>
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
<td><p>General ledger</p></td>
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
<td><p>DimensionAttributeSet</p></td>
</tr>
</tbody>
</table>


## Remarks

After updating the DimensionAttributeSet field with the value of the hash fields in the DimensionAttributeSet table, the HashIdx index is reset not to allow for duplicate records.

  


