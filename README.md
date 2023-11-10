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
Implementation of python code
## Step 4:

Serving the HTML pages.

## Step 5:

Testing the webserver
# PROGRAM:
Type your code here
``````
from http.server inport HTTPServer, BaseHTTPRequestHandler
content = """

<html>
<head>
<title>webservers</title>
</head>
<body>
<h1>Top Five Web Apllication Development Framework</h1>
<h2>1.Django</h2>
<h3>2.MEAN Stack</h3>
<h4>3.React</h4>
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
httpd.serve_forever()
``````

# OUTPUT:
![webserver png](https://github.com/Kamal-Raj-A/webserver/assets/145742556/8e9c0502-e168-4b6b-93d0-c9ff7000d6f1)

# RESULT:

The program is executed succesfully
