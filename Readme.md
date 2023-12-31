# Openldap from sources

### Step 1 - Clone this repository

``git clone https://github.com/codesshaman/docker_openldap_server.git && cd docker_openldap_server``

### Step 2 - Create .env with server data

``cp .env.example .env`` and open .env in text editor,

or use make (unix):

``make env && nano .env``

Change data if necessary.

### Step 3 - launch configuration

``docker-compose up -d --build``

or use make (unix):

``make build``

### Step 4 - Authorize

Open phpldapadmin in ``http://localhost:8081/``

Authorize with admin privileges:

Login: ``cn=admin,dc=local,dc=host``
Passwd: ``admin``

Or yours own data from .env file