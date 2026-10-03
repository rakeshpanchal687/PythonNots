**markdown**

**# Docker Notes**



\## Concepts

\- \*\*Docker:\*\* Docker ek open Source Software platform hai jiska istemal applications Ko develop ship aur Run ke liye kiya Jata Hai.

\- Application aur required environment ko lightweight container me package karta hai.

\- \*\*Image:\*\* Kisi Software ko Docker me chalane ka ready package (Java, Python, Tomcat, Wildfly, Nginx, MySQL).

\- \*\*Dockerfile:\*\* Docker Image banane ke liye file banate hai (isme koi extension nahi hota, `.txt` nahi hona chahiye).



\---



\## **Dockerfile Examples**



**### Tomcat:**

**```dockerfile**



FROM tomcat:10

COPY index.html /usr/local/tomcat/webapps/ROOT/index.html



**Nginx:**

**Dockerfile**



FROM nginx

COPY index.html /usr/share/nginx/html/



**Wildfly:**

**Dockerfile**



FROM quay.io/wildfly/wildfly

COPY ROOT.war /opt/jboss/wildfly/standalone/deployments/ROOT.war



**Docker Commands**

**Build Image:**

docker build -t myapp .



markdown

\# Docker Notes



\## Concepts

\- \*\*Docker:\*\* Docker ek open Source Software platform hai jiska istemal applications Ko develop ship aur Run ke liye kiya Jata Hai.

\- Application aur required environment ko lightweight container me package karta hai.

\- \*\*Image:\*\* Kisi Software ko Docker me chalane ka ready package (Java, Python, Tomcat, Wildfly, Nginx, MySQL).

\- \*\*Dockerfile:\*\* Docker Image banane ke liye file banate hai (isme koi extension nahi hota, `.txt` nahi hona chahiye).



\---



\## Dockerfile Examples



\### Tomcat:

```dockerfile

FROM tomcat:10

COPY index.html /usr/local/tomcat/webapps/ROOT/index.html

Nginx:

Dockerfile

FROM nginx

COPY index.html /usr/share/nginx/html/

Wildfly:

Dockerfile

FROM quay.io/wildfly/wildfly

COPY ROOT.war /opt/jboss/wildfly/standalone/deployments/ROOT.war

Docker Commands

Build Image:

docker build -t myapp .



**Run Nginx/Apache:**

docker run -d -p 8080:80 myapp



**Run Tomcat/WildFly:**

docker run -d -p 8080:8080 myappdocker run -d -p 8080:80 myapp



**Run Tomcat/WildFly:**

docker run -d -p 8080:8080 myapp

