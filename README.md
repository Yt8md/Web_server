# Developing a Simple Webserver
Name: Mathesh
Ref no: 23013902

# AIM:

Develop a webserver to display about top five web application development frameworks.

# DESIGN STEPS:

## Step 1:

HTML content creation is done

## Step 2:

Design of webserver workflow

## Step 3:

Implementation using python code

## Program:
```
from http.server import HTTPserver, BaseHTTPRequestHandler

content = """
<html>
<head>
</head>
<body>
<h1>Name:Mathesh S</h1>
<h1>Departmeant:AI&DS<h2>
</body>
</html>
"""

class HelloHandler(BaseHTTPRequestHandler):
    def do_GET(self):
        self.send_response(200)
        self.send_header('Content-type', 'text/html; character=utf-8')
        self.end_headers()
        self.wfile.write(content.encode())


server_address = ('', 80)
http = HTTPServer(server_address, HelloHandler)
httpd.server_forever()
```

## Step 4:

Serving the HTML pages.
 
## Step 5:

Testing the webserver
# PROGRAM:
Type your code here
# OUTPUT:
![Alt Text](images/webserver1.png)


# RESULT:

The program is executed succesfully
