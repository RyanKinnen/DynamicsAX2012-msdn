﻿---
title: PmfReleaseUpdateDB30.updateBlockedInventBatches Upgrade Script
TOCTitle: PmfReleaseUpdateDB30.updateBlockedInventBatches Upgrade Script
ms:assetid: 14a35435-72bc-bc0f-1a13-3d355e24c8e7
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ718519(v=AX.60)
ms:contentKeyID: 49706801
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# PmfReleaseUpdateDB30.updateBlockedInventBatches Upgrade Script 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2_

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Class</strong></p></td>
<td><p>PmfReleaseUpdateDB30</p></td>
</tr>
<tr class="even">
<td><p><strong>Method</strong></p></td>
<td><p>updateBlockedInventBatches</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Assigns disposition code with unavailable status to the batches that were marked as blocked.</p></td>
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
<td><p>PDS</p></td>
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
<td><p>INVENTBATCH</p></td>
</tr>
<tr class="even">
<td><p>PDSHISTORYINVENTDISPOSITION</p></td>
</tr>
<tr class="odd">
<td><p>PDSDISPOSITIONMASTER</p></td>
</tr>
</tbody>
</table>

  


