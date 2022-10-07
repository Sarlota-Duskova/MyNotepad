# Active Directory

## Windows Domains

The server that runs the Active Directory services is known as a Domain Controller (DC).

**The main advantages of having a configured Windows domain are:**

* **Centralised identity management:** All users across the network can be configured from Active Directory with minimum effort.
* **Managing security policies:** You can configure security policies directly from Active Directory and apply them to users and computers across the network as needed.

## Active Directory

The core of any Windows Domain is the Active Directory Domain Service (AD DS).

* Users
* Machines
  * The machine account name is the computer's name followed by a dollar sign.
* Security Groups

To configure users, groups or machines in Active Directory run "Active Directory Users and Computers" from the start menu:

* These objects are organised in Organizational Units (OUs) which are container objects that allow you to classify users and machines.
* OUs (Organizational Unit) are handy for applying policies to users and computers, which include specific configurations that pertain to sets of users depending on their particular role in the enterprise.
* Security Groups, on the other hand, are used to grant permissions over resources.

## Group police

* Windows manages such policies through Group Policy Objects (GPO).
* GPOs are simply a collection of settings that can be applied to OUs.
* GPOs can contain policies aimed at either users or computers, allowing you to set a baseline on specific machines and identities.
* To configure GPOs, you can use the Group Policy Management tool.

#### GPO distribution

* GPOs are distributed to the network via a network share called SYSVOL, which is stored in the DC.
* All users in a domain should typically have access to this share over the network to sync their GPOs periodically.
* The SYSVOL share points by default to the C:\Windows\SYSVOL\sysvol\ directory on each of the DCs in our network.

## Trees, Forests and Trusts

#### Trees

* If our `thm.local` domain was split into two subdomains for UK and US branches, you could build a tree with a root domain of `thm.local` and two subdomains called `uk.thm.local` and `us.thm.local`, each with its AD, computers and users.

#### Forests

* The union of several trees with different namespaces into the same network is known as a forest.&#x20;

#### Trust Relationships

* Having multiple domains organised in trees and forest allows you to have a nice compartmentalised network in terms of management and resources.
* In simple terms, having a trust relationship between domains allows you to authorise a user from domain `THM UK` to access resources from domain `MHT EU`.
