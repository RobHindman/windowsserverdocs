---
title: Deploy guarded hosts
ms.custom: na
ms.prod: windows-server-threshold
ms.topic: article
ms.assetid: 2379ca26-b32d-4055-8b4b-99d1f2df37e1
manager: dongill
author: rpsqrd
ms.technology: security-guarded-fabric
ms.date: 08/28/2017
---

# Deploy guarded hosts

>Applies to: Windows Server (Semi-Annual Channel), Windows Server 2016

>[!div class="step-by-step"]
[« Deploy HGS](guarded-fabric-setting-up-the-host-guardian-service-hgs.md)
[Deploy shielded virtual machines »](guarded-fabric-configuration-scenarios-for-shielded-vms-overview.md)

The topics in this section describe the steps that a fabric administrator takes to configure Hyper-V hosts to work with the Host Guardian Service (HGS). Before you can start these steps, at least one node in the [HGS cluster must be set up](guarded-fabric-setting-up-the-host-guardian-service-hgs.md).

**For Admin-trusted attestation**:
1. [Configure the fabric DNS](guarded-fabric-configuring-fabric-dns.md): Tells how to set up a DNS forwarder from the fabric domain to the HGS domain.
2. [Create a security group](guarded-fabric-admin-trusted-attestation-creating-a-security-group.md): Tells how to set up an Active Directory security group in the fabric domain, add guarded hosts as members of that group, and provide that group identifier to the HGS administrator. 
3. [Confirm guarded hosts can attest](guarded-fabric-confirm-hosts-can-attest-successfully.md)

**For TPM-trusted attestation**:
1. [Configure the fabric DNS](guarded-fabric-configuring-fabric-dns.md): Tells how to set up a DNS forwarder from the fabric domain to the HGS domain.
2. [Capture information required by HGS](guarded-fabric-tpm-trusted-attestation-capturing-hardware.md): Tells how to capture TPM identifiers (also called platform identifiers), create a Code Integrity policy, and create a TPM baseline. Then you will provide this information to the HGS administrator to configure attestation.
3. [Confirm guarded hosts can attest](guarded-fabric-confirm-hosts-can-attest-successfully.md)

## See also

- [Deployment tasks for guarded fabrics and shielded VMs](guarded-fabric-deploying-hgs-overview.md#deployment-tasks-for-guarded-fabrics-and-shielded-vms)
