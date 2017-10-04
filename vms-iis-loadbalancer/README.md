# 2 VMs with IIS and Load Balancer

<a href="https://portal.azure.com/#create/microsoft.template/uri/https%3a%2f%2fraw.githubusercontent.com%2fdanieldbr%2fazure-arm-templates%2fmaster%2fvms-iis-loadbalancer%2fazuredeploy.json"><img src="http://azuredeploy.net/deploybutton.png"></a>

This ARM template creates:
- 1 Virtual Network
- 1 Subnet
- 1 Public IP with a dynamic IP and random DNS name label
- 1 Load Balancer
- 1 Network Security Group with 2 rules
- 1 Storage Account for VM's disks
- 1 Storage Account for VMs's diagnostics
- 1 Availability Set
- 2 VMs
- DSC extension to install IIS and create a sample HTML file.

Once deployment is finished, check the DNS name at the Public IP address resource and browse that name to see the load balancer in action.

## Note
This ARM template uses unmanaged disks and API versions compatible with Azure Stack.
