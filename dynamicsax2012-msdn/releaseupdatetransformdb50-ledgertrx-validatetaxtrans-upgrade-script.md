﻿---
title: ReleaseUpdateTransformDB50_LedgerTrx.validateTaxTrans Upgrade Script
TOCTitle: ReleaseUpdateTransformDB50_LedgerTrx.validateTaxTrans Upgrade Script
ms:assetid: cc522e7b-5d55-8cb1-5836-7a1942da76b1
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ719695(v=AX.60)
ms:contentKeyID: 49711261
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateTransformDB50\_LedgerTrx.validateTaxTrans Upgrade Script 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2, Microsoft Dynamics AX 2012 Feature Pack, Microsoft Dynamics AX 2012_

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Class</strong></p></td>
<td><p>ReleaseUpdateTransformDB50_LedgerTrx</p></td>
</tr>
<tr class="even">
<td><p><strong>Method</strong></p></td>
<td><p>validateTaxTrans</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Performs validation to make sure that the records in the TaxTrans table have valid values for the AccountNum and Dimension field.</p></td>
</tr>
<tr class="even">
<td><p><strong>Script Type</strong></p></td>
<td><p>Upgrade readiness scripts</p></td>
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
<td><p>LedgerTrans</p></td>
</tr>
<tr class="even">
<td><p></p></td>
</tr>
<tr class="odd">
<td><p></p></td>
</tr>
<tr class="even">
<td><p></p></td>
</tr>
</tbody>
</table>


<table xmlns="http://www.w3.org/1999/xhtml">
              <tr><th colspan="2">
		
   <p>
   
	 Validation Issues
  </p>
  </th></tr>
              <tr><td>
		
   <p>
   
	 
            Validation Issues Description
          
  </p>
  </td><td>
		
   <p>
   
	 There may be a situation where the TaxTrans table contains a record with an invalid value for the AccountNum or Dimension fields. The account and dimension must exist in the LedgerTable table in order for the upgrade to proceed.
  </p>
  </td></tr>
              <tr><td>
		
   <p>
   
	 
            Checked Conditions
          
  </p>
  </td><td>
		
   <p>
   
	 Checks to make sure that the values for the TaxTrans.AccountNum, TaxTrans.OperationAccount, TaxTrans. TaxOffsetAccountUseTax, and TaxTrans. Dimension fields contain values that are found in the LedgerTabletable.
  </p>
  </td></tr>
              <tr><td>
		
   <p>
   
	 
            Mitigation/How-to-fix
          
  </p>
  </td><td>
		
   <p>
   
	 Modify the existing TaxTrans record to hold a valid value for the AccountNum, OperationAccount, TaxOffsetAccountUseTax, and Dimension fields. These values must exist in the LedgerTable table.
  </p>
  </td></tr>
            </table>

  


