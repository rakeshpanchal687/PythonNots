**# Devops (Servers) \& Networking**

\## Networking \& Server Basics

\- \*\*Servers:\*\* Network Per Connected User ya devices Ko data Applications ya Services Provide Karta Hai.

\- \*\*Client:\*\* Service maangta Hai (jaise: Mobile).

\- \*\*Server:\*\* Service deta hai (jaise: YouTube).

\- \*\*Network:\*\* Ek Medium of Communication Hai (jaise: Internet).

\- \*\*URL:\*\* Uniform Resource Locator

\- \*\*Domain Name:\*\* Website ka human Name Hota Hai jo IP address ki jagah use Kiya Jata Hai.

\- \*\*IP Address:\*\* Hotel Ka Naam / Address

\- \*\*Port Number:\*\* Hotel Ka Room Number

 **1. Apache Tomcat**

\- Only Java ke liye or Choti Applications ke liye.

\- \*\*Run:\*\* `Tomcat Root folder` -> Go to `bin` -> Double click on `startup.bat`

\- \*\*Stop:\*\* `Tomcat Root folder` -> Go to `bin` -> Double Click on `shutdown.bat` (Alternative: `Ctrl + C`)

**\- \*\*Port Change:\*\***

 - `conf` directory me jayein

 - `server.xml` ko Notepad me open karein

 - Connector port line find karein (`Ctrl + F`)

 - Port change karein (8080 se 8081)

**\- \*\*HTML File Run:\*\***

 - `webapps` ke andar paste karein

 - Extension check karein (remove `.txt`)

- Run: `localhost:8080/index.html`

**\## 2. Wildfly (JBoss)**

\- Java ke liye or Badi Applications Ke liye.

\- \*\*Run:\*\* `Root Folder` -> `bin` -> Double click on `standalone.bat` (`localhost:8080`)

\- \*\*Stop:\*\* Command Prompt me `Ctrl + C` press karein

**\- \*\*Port Change:\*\***

 - `standalone/configuration` me jayein

 - `standalone.xml` ko Notepad me kholein

 - `socket-binding` line me port change karein

**\- \*\*HTML File Run:\*\***

 - `welcome-content` me file paste karein

 - Run: `localhost:8080/<file\_name>`

**\## 3. Nginx**

\- Frontend Ke liye use Hota Hai (Default Port: 80).

\- \*\*Run:\*\* Root folder CMD me type karein: `start nginx`

\- \*\*Stop:\*\* `nginx -s stop`

\- \*\*Port Change:\*\*

 - `conf/nginx.conf` ko Notepad me kholein

 - `listen 80;` line change karein

 - Reload ke liye: `nginx -s reload`

**\- \*\*HTML File Run:\*\***

 - `html` folder me paste karein

 - Run: `localhost/<file\_name>`


