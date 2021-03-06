﻿---
title: ReleaseUpdateDB60_Invent.allowDupInventProdComLineDetailKeyIdx Upgrade Script
TOCTitle: ReleaseUpdateDB60_Invent.allowDupInventProdComLineDetailKeyIdx Upgrade Script
ms:assetid: 25f2d232-9cd6-f8ec-3201-d846d9200d43
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ685039(v=AX.60)
ms:contentKeyID: 49707239
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateDB60\_Invent.allowDupInventProdComLineDetailKeyIdx Upgrade Script 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2, Microsoft Dynamics AX 2012 Feature Pack, Microsoft Dynamics AX 2012_

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Class</strong></p></td>
<td><p>ReleaseUpdateDB60_Invent</p></td>
</tr>
<tr class="even">
<td><p><strong>Method</strong></p></td>
<td><p>allowDupInventProdComLineDetailKeyIdx</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Updates the KeyIdx index in the InventProdComLineDetail table to allow for duplicate records.</p></td>
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
<td><p>Inventory management</p></td>
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
<td><p>InventProdComLineDetail</p></td>
</tr>
</tbody>
</table>


## Remarks

The InventProdComPeriodId field is replaced with the new surrogate key InventProdComTable field in the unique KeyIdx index. Initially, this field contains no value. So the index is set to allow duplicates before the field is updated with the value of the RecId field of the InventProdComTable table.

  


