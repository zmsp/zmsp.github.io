---
title:  "How to Reset PostgreSQL"
header:
    teaser: "images/til-page.jpg"
categories: 
  - Guide
tags:
  - PostgreSQL
  - Reset
  - Configuration
  - Version
  - Password
  - Security
---

**How to Reset PostgreSQL**

**Title: How to Reset PostgreSQL**

**TLDR:**

If you're looking to reset PostgreSQL, follow these steps:

```
sudo systemctl stop postgresql
sudo -u postgres pg_ctl -D /var/lib/pgsql/data -l logfile start
```

**Checking Database Status:**

To make sure the database is running, use the command:

```
ps aux | grep post
```

**Reset Process Warning:**

Please be cautious! This process will delete all PostgreSQL data and configurations.

**Reset Process Steps:**

1. Replace "X.x" with your PostgreSQL version number.
2. Execute the following commands:

```
sudo systemctl stop postgres-X.x # stops PostgreSQL services  
sudo -u postgres rm –rf /var/lib/pgsql/X.x/data/*
sudo systemctl start postgresql-X.x
```

**Additional Information:**

After the reset, your database connection will be lost until you configure `data/pg_hba.conf`. To allow all connections, add `host all all 192.168.0.0/24 trust` to `/var/lib/pgsql/X.x/data/pg_hba.conf`. This configuration allows connections from the IP range 192.168.0.0 to 192.168.255.255 without credentials.

**Resetting System Password:**

If you only want to reset the system password:

1. Run PostgreSQL as the postgres user:

```
sudo -u postgres psql
```

2. Change the password:

```
\password
```

3. Enter the new password twice and exit:

```
\q
```
