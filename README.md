# navicat remote MySQL connection
26/10/2021 - we updated ntunnel_mysql.php script with [Webcy inc.](https://webcy.ir) for remote connect to MySQL or MariaDB database by [Navicat](http://navicat.com/).
----------
### Older version 
An older version of this script is available at the [@rothkj1022/ntunnel_mysqli](https://github.com/rothkj1022/ntunnel_mysqli). But that version does not support PHP8.
### New version 
**We updated it and it is now available for PHP8 in [@imseyed/navicat_remote_MySQL](https://github.com/imseyed/navicat_remote_MySQL/).**

----------

# Remote MySQL
If you are using a shared host and the remoteSQL is blocked, you will need this script to access the database through navicat.
Both versions Navicat Premium 15 and Navicat 15 for MySQL support this script.

## About Tunneling
HTTP Tunneling is a method for connecting to a server that uses the same protocol (http(s)://) as a webserver does. It is used while your ISPs do not allow direct connections to database, but allows establishing HTTP connections.

## Uploading the Tunneling Script

To set up an HTTP tunnel, first upload the ntunnel_mysqli.php script to your web server.

## Setting up HTTP Tunnel

The following instruction guides you through the process of configuring a HTTP connection.

1. Select the HTTP tab in Navicat and enable **Use HTTP Tunnel**.
2. Enter URL of the tunneling script, e.g. *http://www.example.com/ntunnel_mysqli.php* .
3. If your server installed a Web Application Firewall, you can check the **Encode outgoing query with base64** option.
4. If the tunneling script is hosted in a password protected server or you have to access internet over a proxy server, you can provide the required authentication details in **Authentication** or **Proxy** tab.
5. Navicat host name at the General settings page should be set relatively to the HTTP server which provided by your database hosting company.
