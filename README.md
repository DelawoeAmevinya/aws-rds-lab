# Building and Connecting an Amazon RDS Database

I completed a hands-on lab where I:
- Launched an **Amazon RDS DB instance with Multi-AZ (high availability)**
- Configured **security groups** to securely connect my web server to the database
- Tested the setup with a **successful DB connection**
- Integrated the DB into a **web application** and performed CRUD operations

## LinkedIn post
(Original post published on LinkedIn)
> I recently completed a hands-on lab where I launched a Multi-AZ Amazon RDS, configured secure access via security groups, and connected a web app to perform CRUD operations. Seeing the app interact with the RDS instance in real time was a great way to connect theory with practice.

**LinkedIn post URL:** https://www.linkedin.com/posts/your-link-here

## Screenshots
![RDS Dashboard](screenshots/rdsdashboard.png)  
*RDS Dashboard showing Multi-AZ instance*

![Security Group](screenshots/securitygroup.png)  
*Security Group inbound rules allowing web server access*

![Connection Test](screenshots/connectiontest.png)  
*Successful DB connection test via client/CLI*

![Web App](screenshots/webapplication.png)  
*Web app displaying data retrieved from RDS*

## What I did (short steps)
1. Launched RDS instance (Multi-AZ) in AWS RDS.
2. Created/updated security group to allow the web server’s IP/port.
3. Tested DB connectivity with a client (e.g., MySQL Workbench / psql).
4. Configured the web app connection string (using env var).
5. Performed CREATE/READ/UPDATE/DELETE operations through the app.

## Notes & security
- **Never commit** credentials, `.env` files, or private keys.  
- This repo excludes secrets — keep them in environment variables or a secrets manager.

## License
Choose a license (e.g., MIT) — or add one via GitHub when creating the repo.
