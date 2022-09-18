# architecture
## Public Load Balancer
HTTPS requests from external users, such as users of Hyperion Financial Reporting Web Studio, flow through the internet gateway that's attached to the VCN in currently active region. The requests then pass through the global Oracle Cloud Infrastructure Web Application Firewall (WAF) service, which protects the applications from malicious and unwanted internet traffic. Traffic that passes the WAF rules is forwarded to the public load balancer. The load balancer terminates SSL/TSL, and distributes HTTP requests to the private web tier.
## Private Load Balancer
Traffic from your internal and on-premises users flows through IPSec VPN tunnels or FastConnect virtual circuits to the dynamic routing gateway (DRG) that's attached to the VCN. A private load balancer intercepts the requests and distributes them to the private web tier.
## Region
An Oracle Cloud Infrastructure region is a localized geographic area that contains one or more data centers, called availability domains. Regions are independent of other regions, and vast distances can separate them (across countries or even continents)
## Availability domain
Availability domains are standalone, independent data centers within a region. The physical resources in each availability domain are isolated from the resources in the other availability domains, which provides fault tolerance. Availability domains don’t share infrastructure such as power or cooling, or the internal availability domain network. So, a failure at one availability domain is unlikely to affect the other availability domains in the region.
## Fault domain
A fault domain is a grouping of hardware and infrastructure within an availability domain. Each availability domain has three fault domains with independent power and hardware. When you distribute resources across multiple fault domains, your applications can tolerate physical server failure, system maintenance, and power failures inside a fault domain.
## Network address translation (NAT) gateway
A NAT gateway enables private resources in a VCN to access hosts on the internet, without exposing those resources to incoming internet connections.

## Service gateway
The service gateway provides access from a VCN to other services, such as Oracle Cloud Infrastructure Object Storage, Autonomous database.  The traffic from the VCN to the Oracle service travels over the Oracle network fabric and never traverses the internet.
## Block storage
With block storage volumes, you can create, attach, connect, and move storage volumes, and change volume performance to meet your storage, performance, and application requirements. After you attach and connect a volume to an instance, you can use the volume like a regular hard drive. You can also disconnect a volume and attach it to another instance without losing data.
## Autonomous Transaction Processing
Oracle Autonomous Transaction Processing is a self-driving, self-securing, self-repairing database service that is optimized for transaction processing workloads. You do not need to configure or manage any hardware, or install any software. Oracle Cloud Infrastructure handles creating the database, as well as backing up, patching, upgrading, and tuning the database
## Dynamic routing gateway (DRG)
The DRG is a virtual router that provides a path for private network traffic between a VCN and a network outside the region, such as a VCN in another Oracle Cloud Infrastructure region, an on-premises network, or a network in another cloud provider.
## Container Engine for Kubernetes
Oracle Cloud Infrastructure Container Engine for Kubernetes is a fully managed, scalable, and highly available service that you can use to deploy your containerized applications to the cloud. You specify the compute resources that your applications require, and Container Engine for Kubernetes provisions them on Oracle Cloud Infrastructure in an existing tenancy. Container Engine for Kubernetes uses Kubernetes to automate the deployment, scaling, and management of containerized applications across clusters of hosts.

## Container Registry
Oracle Cloud Infrastructure Registry is an Oracle-managed registry that enables you to simplify your development-to-production workflow. Registry makes it easy for you to store, share, and manage development artifacts, like Docker images. The highly available and scalable architecture of Oracle Cloud Infrastructure ensures that you can deploy and manage your applications reliably.
## Logging Analytics
Logging Analytics is a fully managed SaaS regional service available in more than 27 regions that provides collection, indexing, enrichment, query, visualization, and alerting for logs from any IT component running on on-premises, OCI or 3rd party cloud.
## Kubernetes Application Pods
## Kubernetes Daemonsets
## Kubernetes PV, PVC & SC
## Kubernetes Ingress
## Kubernetes Service
## Kubernetes Monitoring Pods
