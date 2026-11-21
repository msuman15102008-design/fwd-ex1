# Ex02 Django ORM Web Application
## Date:15-11-2026 
## REG NO:26018167
## AIM
To develop a Django Application to store and retrieve data from a E-Commerce Website Database for Amazon or Flipkart using Object Relational Mapping(ORM).


## ENTITY RELATIONSHIP DIAGRAM



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
~~~
from http.server import HTTPServer, BaseHTTPRequestHandler
content = """
<!DOCTYPE html>
<html>
<head>
    <title>List of Protocols</title>
</head>
<body>

    <h2>List of Network Protocols</h2>

    <ol>
        <li>HTTP</li>
        <li>HTTPS</li>
        <li>FTP</li>
        <li>TCP</li>
        <li>IP</li>
        <li>SMTP</li>
        <li>POP3</li>
        <li>DNS</li>
        <li>SSH</li>
        <li>Telnet</li>
    </ol>

</body>
</html>
"""
class myhandler(BaseHTTPRequestHandler):
    def do_GET(self):
        print("request received")
        self.send_response(200)
        self.send_header('content-type', 'text/html; charset=utf-8')
        self.end_headers()
        self.wfile.write(content.encode())
server_address = ('',880)
httpd = HTTPServer(server_address,myhandler)
print("my webserver is running...")
httpd.serve_forever()
~~~

## OUTPUT
![alt text](<myapp/first/Screenshot 2026-11-16 181358.png>)
![alt text](<Screenshot 2026-11-14 160647.png>)
## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
