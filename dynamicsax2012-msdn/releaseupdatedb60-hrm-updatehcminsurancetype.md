﻿---
title: ReleaseUpdateDB60_HRM.updateHcmInsuranceType
TOCTitle: ReleaseUpdateDB60_HRM.updateHcmInsuranceType
ms:assetid: f8936e70-a1ae-0b19-2eb0-7a2952583ddb
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ737647(v=AX.60)
ms:contentKeyID: 49712341
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateDB60\_HRM.updateHcmInsuranceType 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2_

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Class</strong></p></td>
<td><p>ReleaseUpdateDB60_HRM</p></td>
</tr>
<tr class="even">
<td><p><strong>Method</strong></p></td>
<td><p>updateHcmInsuranceType</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Inserts records into the &lt;c&gt;HcmInsuranceType&lt;/c&gt; table from the &lt;c&gt;HRMInsuranceType&lt;/c&gt; table.</p></td>
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
<td><p>Human Resources</p></td>
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
<td><p>HcmInsuranceType</p></td>
</tr>
<tr class="even">
<td><p>HRMInsuranceType</p></td>
</tr>
</tbody>
</table>


## Remarks

This upgrade will discard duplicate records if the \<c\>HrmInsuranceTypeId\</c\> field and the \<c\>Description\</c\> field of the \<c\>HRMInsuranceType\</c\> table are identical. The new unique identifier \<c\>InsuranceTypeId\</c\> field of the \<c\>HcmInsuranceType\</c\> table combines the \<c\>HrmInsuranceTypeId\</c\> field and the \<c\>DataAreaId\</c\> field of the \<c\>HRMInsuranceType\</c\> table from the first record found. All records found that are identified as duplicates in other companies will be discarded. If only one company exists, the \<c\>DataAreaId\</c\> field will not be appended.

## Data Migration Section

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>From Table: HRMInsuranceType</p></th>
<th><p>To Table: HcmInsuranceType</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p></p></td>
<td><p></p></td>
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
<td><p>HcmInsuranceType</p></td>
<td><p></p></td>
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
<td><p>HRMInsuranceType</p></td>
<td><p>*</p></td>
</tr>
</tbody>
</table>

  


