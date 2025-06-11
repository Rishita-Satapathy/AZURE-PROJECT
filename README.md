1. Create separate virtual networks for a database (backend) and frontend of application, respectively.
2. Deploy Virtual Machines for hosting the front end of the application and database. Connect it with a jump Vm or server to make changes to the frontend or backend
3. Apply load balancer to the frontend servers in the frontend network and attach public IP to load balancer only.
4. Enable autoscaling for managing the traffic
5. Connect to the VMs through a private path setup by the jump servers. (Use VPN)
6. Deploy it with Azure Hosting service and map public IP of load balancer to the domain name
7. Perform the operations from the frontend as a general user and check the results in the database
8. Apply an SSL certificate to the domain while it is hosted
