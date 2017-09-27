# Active Directoy with VM joining the domain

Samples templates to create an Active Directoy deployment, with windows VMs joininig the domain and Linux VMs in the same virtual network.
 * All virtual machines have private static IPs
 * Virtual Network is peered to an existing virtual network (in a different resource group)
 
**Note - This is still work in progress**

1. [ad-new-domain.json](ad-new-domain.json) - create a new Vnet, a new Windows VM and a new AD Forest, Domain and DC
2. [new-vm-join-domain.json](new-vm-join-domain.json) - create a new windows VM and add it to an existing Vnet, subnet and doamin
3. [existing-vnet-peering.json](existing-vnet-peering.json) - create peering between VNet in the resource group, and a Vnet in a different resource group. **Note - this template should be deployed on both VNets. Each time from the resource group the VNet resides in**
