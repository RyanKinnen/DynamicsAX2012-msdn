﻿---
title: ReleaseUpdateDB60_Ledger.updateTaxServiceCodeDescription_BR Upgrade Script
TOCTitle: ReleaseUpdateDB60_Ledger.updateTaxServiceCodeDescription_BR Upgrade Script
ms:assetid: b56ef66e-aa9f-4b70-7b65-113cc210ddee
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ737001(v=AX.60)
ms:contentKeyID: 49710683
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateDB60\_Ledger.updateTaxServiceCodeDescription\_BR Upgrade Script 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2_

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
<td><p>updateTaxServiceCodeDescription_BR</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Updates &lt;c&gt;Description&lt;/c&gt; field of &lt;c&gt;TaxServiceCode_BR&lt;/c&gt; table.</p></td>
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
<td><p>TaxServiceCode_BR</p></td>
</tr>
</tbody>
</table>


## Data Migration Section

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>From Table: TaxServiceCode_BR</p></th>
<th><p>To Table: TaxServiceCode_BR</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>DEL_Description</p></td>
<td><p>Description</p></td>
</tr>
</tbody>
</table>

  


