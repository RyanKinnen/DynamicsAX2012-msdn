﻿---
title: ReleaseUpdateTransformDB41_Prod.validateIfMultisiteActivated Upgrade Script
TOCTitle: ReleaseUpdateTransformDB41_Prod.validateIfMultisiteActivated Upgrade Script
ms:assetid: 2078fbd1-e4f9-7152-494b-f93c5fde4d74
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ684894(v=AX.60)
ms:contentKeyID: 49707096
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateTransformDB41\_Prod.validateIfMultisiteActivated Upgrade Script 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2, Microsoft Dynamics AX 2012 Feature Pack, Microsoft Dynamics AX 2012_

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Class</strong></p></td>
<td><p>ReleaseUpdateTransformDB41_Prod</p></td>
</tr>
<tr class="even">
<td><p><strong>Method</strong></p></td>
<td><p>validateIfMultisiteActivated</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Validates if the multisite has been activated in all companies.</p></td>
</tr>
<tr class="even">
<td><p><strong>Script Type</strong></p></td>
<td><p>Upgrade readiness scripts</p></td>
</tr>
<tr class="odd">
<td><p><strong>Microsoft Dynamics AX Source</strong></p></td>
<td><p>UNKNOWN VERSION</p></td>
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
<td><p>Production</p></td>
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
   
	 Validates if the multisite has to be activated in all companies.
  </p>
  </td></tr>
              <tr><td>
		
   <p>
   
	 
            Checked Conditions
          
  </p>
  </td><td>
		
   <p>
   
	 The value of the InventParameters.MultisiteActivated field in all the company accounts.
  </p>
  </td></tr>
              <tr><td>
		
   <p>
   
	 
            Mitigation/How-to-fix
          
  </p>
  </td><td>
		
   <p>
   
	 Activate the multisite in all companies by using the Multisite Activation Wizard.
  </p>
  </td></tr>
            </table>

  


