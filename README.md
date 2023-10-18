# Developing a Simple Webserver
Name: Kamal raj
Ref no: 23012941

# AIM:

Develop a webserver to display about top five web application development frameworks.

# DESIGN STEPS:

## Step 1:

HTML content creation is done

## Step 2:

Design of webserver workflow

## Step 3:
``````
from http.server inport HTTPServer, BaseHTTPRequestHandler
content = """

content = """
<html>
<head>
<title>Student Details</title>
</head>
<body>
<h1>Name:Sai Vishal</h1>
<h1>Department:AI&DS</h1>
<h1>Reference Number:23013576<h1>
</body>
</html>
"""

class HelloHandler(BaseHTTPRequestHandler):
    def do_GET(self):
        self.send_response(200)
        self.send_header('Content-type', 'text/html; charset=utf-8')
        self.end_headers()
        self.wfile.write(content.encode())

server_address = ('', 80)
httpd = HTTPServer(server_address, HelloHandler)
httpd.serve_forever()``````

## Step 4:

Serving the HTML pages.

## Step 5:

Testing the webserver
# PROGRAM:
Type your code here
# OUTPUT:
![Alt Text](https://github.com/Kamal-Raj-A/webserver/blob/main/images/webserver1.png)

# RESULT:

The program is executed succesfully
