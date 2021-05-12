# NextCloud
## Project Overview
Azure deployment of a public load balancer with two Linux VMs running Nextcloud as web front ends and a Linux VM with MariaDB/Mysql as a database. 
## Services Used
- Public Load balancer to allow access to Nextcloud from anywhere.
- Two linux VMs to act as front ends for high availability.
- One linux VM to act as the database backend so data is all in once spot and doesn't need to be syned between two machiens.
- Virtual Network to keep the two web front ends together.
- Storage account to allow for serial connection to the VMs. 
- Availaibility set to allow for easy expansion of web front ends if necessary.
- Apache2 for web hosting service.
- Certbot to give the web host certificates for a secure access to Nextcloud. 
## Future Revisions
- Create real automation for the configuration of the VMs. 
- Create automation for the creating database users. 
## Deployment
1. Deploy the Loadbalancetemplate.json on Azure.
2. Setup the database backend first using the BackendDB text file. (Run each command one at a time and follow comments as some of them require you to modify files and change information from the commands.)
3. Setup both front ends using FrontEnds text file. (Run each command one at a time and follow comments as some of them require you to modify files and change information from the commands.) 
## Data Flow and Visual Diagaram
![NextCloud Framework (1)](https://user-images.githubusercontent.com/35178560/117900785-f8dd7180-b297-11eb-8dfc-72e6cd47ed23.png)



