﻿---
title: ReleaseUpdateDB60_Cust.updateCustDimensions_RU Upgrade Script
TOCTitle: ReleaseUpdateDB60_Cust.updateCustDimensions_RU Upgrade Script
ms:assetid: bc83aff6-4ce4-79f2-baa0-0aac5a2ab905
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ686645(v=AX.60)
ms:contentKeyID: 49710853
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateDB60\_Cust.updateCustDimensions\_RU Upgrade Script 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2, Microsoft Dynamics AX 2012 Feature Pack, Microsoft Dynamics AX 2012_

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Class</strong></p></td>
<td><p>ReleaseUpdateDB60_Cust</p></td>
</tr>
<tr class="even">
<td><p><strong>Method</strong></p></td>
<td><p>updateCustDimensions_RU</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Transforms data from the dimension related fields in the CustParameters and SalesBookVATProcessParameters_RU tables.</p></td>
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
<td><p>Lean Manufacturing</p></td>
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
<td><p>CustParameters</p></td>
</tr>
<tr class="even">
<td><p>SalesBookVATProcessParameters_RU</p></td>
</tr>
</tbody>
</table>


## Remarks

This upgrade is required in order to convert account and dimension data to the new accounts and dimension model for Microsoft Dynamics AX 2012.

## Data Migration Section

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>From Table: CustParameters</p></th>
<th><p>To Table: CustParameters</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>rTax25UnrealisedExpenseAcct</p></td>
<td><p>rTax25UnrealisedExpenseLedgerDimension</p></td>
</tr>
<tr class="even">
<td><p>rTax25BadDebtReserveAcct</p></td>
<td><p>rTax25BadDebtReserveLedgerDimension</p></td>
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
<th><p>From Table: SalesBookVATProcessParameters_RU</p></th>
<th><p>To Table: SalesBookVATProcessParameters_RU</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>LedgerAccount</p></td>
<td><p>LedgerDimension</p></td>
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
<td><p>CustParameters</p></td>
<td><p>rTax25UnrealisedExpenseLedgerDimension</p></td>
<td><p>LedgerDimensionDefaultAccount</p></td>
</tr>
<tr class="even">
<td><p>CustParameters</p></td>
<td><p>rTax25BadDebtReserveLedgerDimension</p></td>
<td><p>LedgerDimensionDefaultAccount</p></td>
</tr>
<tr class="odd">
<td><p>SalesBookVATProcessParameters_RU</p></td>
<td><p>LedgerDimension</p></td>
<td><p>LedgerDimensionDefaultAccount</p></td>
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
<td><p>CustParameters</p></td>
<td><p>rTax25UnrealisedExpenseAcct</p></td>
</tr>
<tr class="even">
<td><p>CustParameters</p></td>
<td><p>rTax25BadDebtReserveAcct</p></td>
</tr>
<tr class="odd">
<td><p>SalesBookVATProcessParameters_RU</p></td>
<td><p>LedgerAccount</p></td>
</tr>
</tbody>
</table>

  


