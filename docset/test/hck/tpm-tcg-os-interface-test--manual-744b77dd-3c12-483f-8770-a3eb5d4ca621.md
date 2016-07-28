---
author: joshbax-msft
title: TPM TCG OS Interface Test (Manual)
description: TPM TCG OS Interface Test (Manual)
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 58526eb6-a9c2-498a-9c93-ed4b67dbe967
---

# TPM TCG OS Interface Test (Manual)


This test validates that the integration of the Trusted Platform Module (TPM) on the system motherboard meets the BitLocker Drive Encryption feature requirements for Windows.

This test is run after a full boot and exercises the TPM and BIOS base, including taking ownership of the TPM, but excluding the setting of physical presence and ACPI interfaces. ACPI physical presence requests to Force Clear, Enable, and Activate the TPM are made both at the beginning (Setup phase) and end (Cleanup phase) of the test, requiring the test operator to be present to accept the requests.

## Test details


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Associated requirements</strong></p></td>
<td><p>System.Fundamentals.TrustedPlatformModule.Windows7SystemsTPM</p>
<p>[See the system hardware requirements.](http://go.microsoft.com/fwlink/p/?linkid=254482)</p></td>
</tr>
<tr class="even">
<td><p><strong>Platforms</strong></p></td>
<td><p>Windows 7 (x64) Windows 7 (x86) Windows Server 2008 R2 (x64)</p></td>
</tr>
<tr class="odd">
<td><p><strong>Expected run time</strong></p></td>
<td><p>~30 minutes</p></td>
</tr>
<tr class="even">
<td><p><strong>Categories</strong></p></td>
<td><p>Certification</p></td>
</tr>
<tr class="odd">
<td><p><strong>Type</strong></p></td>
<td><p>Manual</p></td>
</tr>
</tbody>
</table>

 

## Running the test


Before you run the test, review the prerequisites in [TPM System Fundamentals Testing Prerequisites](tpm-system-fundamentals-testing-prerequisites.md).

This test has no additional parameters.

If BitLocker is enabled on the test machine, it should be disabled before running this test. If TPM was initialized (current status says ownership has been taken), you must: (a) Clear the TPM and then (b) Turn On the TPM. Both actions will require a reboot and approval of the TPM state change during reboot. This test may not resume automatically after going into S4 state (Hibernate), in which case you must restart the machine.

## Troubleshooting


For troubleshooting information, see [Troubleshooting System Fundamentals Testing](troubleshooting-system-fundamentals-testing.md).

Wake up the system manually if it fails to wake up automatically within 5 minutes.

This test returns Pass or Fail. To review test details, review the test log from Windows Hardware Certification Kit (Windows HCK) Studio. To provide more information for troubleshooting failures in this test, you can enable tracing of the TPM. Refer to the steps provided under the Troubleshooting section in [TCG TPM Integration Test (Manual)](tcg-tpm-integration-test--manual-ac56901f-0f66-4013-b156-fe4b036cce60.md). Investigations also need log files with name like ‘tpm\*.txt’ and console.txt from the ‘Documents’ folder

To provide more information for troubleshooting failures in this test, you can enable tracing of the TPM. Refer to the steps provided in the [TCG TPM Integration Test (Manual)](tcg-tpm-integration-test--manual-ac56901f-0f66-4013-b156-fe4b036cce60.md).

 

 





