---
author: joshbax-msft
title: MachinePool Methods
description: MachinePool Methods
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 5596b5d5-a303-4855-a60e-d2f457c54b04
---

# MachinePool Methods


## Public Methods


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>CreateChildPool</strong></p></td>
<td><p>This method creates a child machine pool.</p></td>
</tr>
<tr class="even">
<td><p><strong>DeleteChildPool</strong></p></td>
<td><p>This method deletes a child machine pool that doesn't contain any machines in it.</p></td>
</tr>
<tr class="odd">
<td><p><strong>DeleteMachine</strong></p></td>
<td><p>This method deletes the named machine for this machine pool. The machine to be deleted must be a child machine of this pool. Using the <strong>DeleteMachine</strong> method is NOT recommended because it may leave the deleted machine in an unusable state.</p></td>
</tr>
<tr class="even">
<td><p><strong>Equals</strong></p></td>
<td><p>Overloaded. Overridden.</p></td>
</tr>
<tr class="odd">
<td><p><strong>GetChildPools</strong></p></td>
<td><p>This method retrieves the enumerable list of child machine pools for this machine pool.</p></td>
</tr>
<tr class="even">
<td><p><strong>GetHashCode</strong></p></td>
<td><p>Overridden. This method retrieves (creates) the hash code for a <strong>MachinePool</strong> object.</p></td>
</tr>
<tr class="odd">
<td><p><strong>GetMachines</strong></p></td>
<td><p>This method retrieves the enumerable list of machines contained by this machine pool.</p></td>
</tr>
<tr class="even">
<td><p><strong>GetType</strong></p></td>
<td><p>(Inherited from Object)</p></td>
</tr>
<tr class="odd">
<td><p><strong>MoveMachineTo</strong></p></td>
<td><p>This method moves a machine from one machine pool to another. Moving resource to the root pool will cause an exception.</p></td>
</tr>
<tr class="even">
<td><p><strong>Equality</strong></p></td>
<td><p>This method acts as an Equality operator. The method always returns <strong>false</strong> if either operand is <strong>null</strong>; otherwise, returns <strong>true</strong> or <strong>false</strong>.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Inequality</strong></p></td>
<td><p>This method acts as an Inequality operator. The method always returns <strong>false</strong> if either operand is <strong>null</strong>; otherwise, returns <strong>true</strong> or <strong>false</strong>.</p></td>
</tr>
<tr class="even">
<td><p><strong>ToString</strong></p></td>
<td><p>(Inherited from <strong>Object</strong>)</p></td>
</tr>
<tr class="odd">
<td><p><strong>SetConfiguration Method</strong></p></td>
<td><p>This method sets the configuration for all machines in the machine pool. It also sets the configuration for all machines in the child pools</p></td>
</tr>
</tbody>
</table>

 

## Protected Methods


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>Finalize</strong></p></td>
<td><p>(Inherited from <strong>Object</strong>)</p></td>
</tr>
<tr class="even">
<td><p><strong>MemberwiseClone</strong></p></td>
<td><p>(Inherited from <strong>Object</strong>)</p></td>
</tr>
</tbody>
</table>

 

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_hck\p_hck%5D:%20MachinePool%20Methods%20%20RELEASE:%20%284/27/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")



