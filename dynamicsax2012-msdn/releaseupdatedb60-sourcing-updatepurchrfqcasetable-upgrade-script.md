﻿---
title: ReleaseUpdateDB60_Sourcing.updatePurchRFQCaseTable Upgrade Script
TOCTitle: ReleaseUpdateDB60_Sourcing.updatePurchRFQCaseTable Upgrade Script
ms:assetid: 57774e6b-c921-7696-d45d-d1d4a1af967e
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ736229(v=AX.60)
ms:contentKeyID: 49708404
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateDB60\_Sourcing.updatePurchRFQCaseTable Upgrade Script 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2, Microsoft Dynamics AX 2012 Feature Pack, Microsoft Dynamics AX 2012_

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Class</strong></p></td>
<td><p>ReleaseUpdateDB60_Sourcing</p></td>
</tr>
<tr class="even">
<td><p><strong>Method</strong></p></td>
<td><p>updatePurchRFQCaseTable</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Updates the &lt;c&gt;PurchRFQCaseTable&lt;/c&gt; fields 'Requester', 'ResponsibleWorkerId' with the worker corresponding to the emplId of the previous data. Updates the &lt;c&gt;PurchRFQCaseTable&lt;/c&gt; table field 'ExpiryDateTime' with the ExpiryDate using a default time offset.</p></td>
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
<td><p>SRM</p></td>
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
<td><p>PurchRFQCaseTable</p></td>
</tr>
</tbody>
</table>

  


