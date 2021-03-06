﻿---
title: ReleaseUpdateTransformDB50_Basic.updateTaxIntraCommTable_NL Upgrade Script
TOCTitle: ReleaseUpdateTransformDB50_Basic.updateTaxIntraCommTable_NL Upgrade Script
ms:assetid: c41bae90-1bdb-c336-4dbd-00753b2e2b8b
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ686859(v=AX.60)
ms:contentKeyID: 49711056
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateTransformDB50\_Basic.updateTaxIntraCommTable\_NL Upgrade Script 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2, Microsoft Dynamics AX 2012 Feature Pack, Microsoft Dynamics AX 2012_

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Class</strong></p></td>
<td><p>ReleaseUpdateTransformDB50_Basic</p></td>
</tr>
<tr class="even">
<td><p><strong>Method</strong></p></td>
<td><p>updateTaxIntraCommTable_NL</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Updates the postal address in the TaxIntraCommTable_NL table.</p></td>
</tr>
<tr class="even">
<td><p><strong>Script Type</strong></p></td>
<td><p>Preprocessing 60: Live</p></td>
</tr>
<tr class="odd">
<td><p><strong>Microsoft Dynamics AX Source</strong></p></td>
<td><p>Microsoft Dynamics AX 4.0</p>
<p>Microsoft Dynamics AX 2009</p></td>
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
<td><p>Basic</p></td>
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
<td><p>TaxIntraCommTable_NL</p></td>
</tr>
</tbody>
</table>


## Remarks

This upgrade is required in order to convert postal address data to the new logistics postal address model for Microsoft Dynamics AX 2012. The location for the TaxIntraCommTable\_NL table will be kept as a reference to the LogisticsLocation record.

## Data Migration Section

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>From Table: TaxIntraCommTable_NL</p></th>
<th><p>To Table: LogisticsPostalAddress</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>ContactAddress</p></td>
<td><p>Address</p></td>
</tr>
<tr class="even">
<td><p>ContactCity</p></td>
<td><p>City</p></td>
</tr>
<tr class="odd">
<td><p>ContactZipCode</p></td>
<td><p>ZipCode</p></td>
</tr>
</tbody>
</table>


<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>From Table: LogisticsPostalAddress</p></th>
<th><p>To Table: Shadow_TaxIntraCommTable_NL</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Location</p></td>
<td><p>ContactLocation</p></td>
</tr>
</tbody>
</table>


## New Tables or Fields

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Table</p></th>
<th><p>Field</p></th>
<th><p>Extended Data Type</p>
<p>-or- Base Enum</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>TaxIntraCommTable_NL</p></td>
<td><p>ContactLocation</p></td>
<td><p></p></td>
</tr>
</tbody>
</table>


## Deleted Tables or Fields

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Table</p></th>
<th><p>Field</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>TaxIntraCommTable_NL</p></td>
<td><p>ContactAddress</p></td>
</tr>
<tr class="even">
<td><p>TaxIntraCommTable_NL</p></td>
<td><p>ContactCity</p></td>
</tr>
<tr class="odd">
<td><p>TaxIntraCommTable_NL</p></td>
<td><p>ContactZipCode</p></td>
</tr>
</tbody>
</table>

  


