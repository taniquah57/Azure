# Azure Virtual Machine & Access Management Lab

1. Network Security Group (NSG) – IP Filtering

A Network Security Group (NSG) controls inbound and outbound network traffic to Azure resources.

I explored how to create an inbound security rule that allows traffic from a trusted public IP address while restricting traffic from other IP addresses.

Example configuration:
- Source: My trusted public IP address
- Action: Allow
- Protocol/Port:Based on the required connection
- Purpose: Restrict which IP addresses can communicate with the virtual machine.

Azure NSGs also have default security rules that deny inbound traffic that is not otherwise permitted. Rule priorities determine which rules take effect.

2. Stopping a Virtual Machine (VM)

Stopping a virtual machine helps manage resource usage and costs.

Steps:
1. Open the Azure Portal.
2. Navigate to Virtual Machines.
3. Select the virtual machine.
4. Click Stop.

When stopped and deallocated, the VM releases its compute resources. Storage charges may still apply.

3. Different Ways to Connect to an Azure VM

Azure supports different connection methods depending on the operating system and configuration.

- RDP (Remote Desktop Protocol):** Used to connect to Windows virtual machines.
- SSH (Secure Shell):** Used to connect to Linux virtual machines.
- Azure Bastion:** Allows secure browser-based connections without exposing the VM's public IP address for management access.

These connection methods allow administrators and authorized users to remotely manage virtual machines.

4. Adding Role Assignments – Azure RBAC

Role-Based Access Control (RBAC) allows administrators to control who has access to Azure resources and what actions they can perform.

Steps:
1. Select Add role assignment.
2. Choose an appropriate role.
3. Select a user, group, or service principal.
4. Assign the appropriate permissions.
5. Save the assignment.

RBAC helps organizations manage access according to job responsibilities and the principle of least privilege.

5. Azure Portal Notifications

During the exercise, I observed that a portal notification or setup banner disappeared after adding a user.

This demonstrated how the Azure Portal updates its interface after certain configuration steps. The actual role assignment should still be verified under Access Control (IAM).

6. How I Plan to Use RBAC

I plan to use Role-Based Access Control (RBAC) in my technical portfolio to demonstrate how organizations manage employee access based on job roles and responsibilities.

This includes:
- Creating and managing user accounts.
- Assigning permissions based on job responsibilities.
- Applying the principle of least privilege.
- Ensuring employees only have access to the resources necessary to perform their jobs.

7. Key Takeaways

This lab helped me understand how Azure supports network security, virtual machine management, remote connectivity, and identity and access management.
I gained a better understanding of how administrators can restrict network traffic, manage cloud resources, and control user permissions within an organization.
