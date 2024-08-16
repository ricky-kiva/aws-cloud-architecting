1. Make VPC (ho-db-dcd)
2. Make cust. private subnet (ho-db-dcd-subnet-private2-ap-southeast-1b)
3. Make public security group for EC2 (ho-db-dcd-securitygroup)
4. Make private security group for DB instance (ho-db-dcd-db-securitygroup)
5. Make RDS DB Subnet Group (ho-db-dcd-db-subnet-group)

6. Create MariaDB DB (ho-db-dcd-db-instance-1)

7. Create EC2 Instance (ho-db-dcd-web-server)
8. Connect to the EC2 Instance
- Update the softwares
- Install server packages (this: LAMP stack)
- Install web server (this: Apache)
- Start web server
9. Check Web Server by opening the: Public IPv4 DNS
11. Enable Web Server every system boot
12. Allow EC2 user manage root dir. files (on: `/var/www`) 
- Make "www" group
- Add user to the group (user: ec2-user)
- Refresh configuration by EXIT
13. Re-connect to EC2 Instance
14. Update user permission on `/var/www` dir.
- Change the group that manage `/var/www`
- Change `/var/www` permissions
15. Make `dbinfo.inc` on `/var/www/inc`
16. Make index page on `/var/www/html` (this n: SamplePage.php)
17. Restart web server

18. Check your website by url (Public-IPv4-DNS/index_file)