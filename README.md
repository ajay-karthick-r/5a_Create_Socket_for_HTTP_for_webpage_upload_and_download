# 5a_Create_Socket_for_HTTP_for_webpage_upload_and_download
## AIM :
To write a PYTHON program for socket for HTTP for web page upload and download
## Algorithm

1.Start the program.
<BR>
2.Get the frame size from the user
<BR>
3.To create the frame based on the user request.
<BR>
4.To send frames to server from the client side.
<BR>
5.If your frames reach the server it will send ACK signal to client otherwise it will send NACK signal to client.
<BR>
6.Stop the program
<BR>
## Program 
```
import webbrowser
import os

def download_and_open():

    html = """
<!DOCTYPE html>
<html>
<head>
    <title>Socket HTTP Experiment</title>
</head>

<body>

<h1>Welcome to Socket Programming Lab</h1>

<h2>Experiment No. 5</h2>

<p>
This webpage is created for HTTP socket upload and download experiment.
</p>

<h3>Student Details</h3>

<ul>
<li>Name : Ajay karthick</li>
<li>Department : AIDS</li>
<li>College : Saveetha Engineering College</li>
</ul>

</body>
</html>
"""

    filename = "page.html"

    with open(filename, "w", encoding="utf-8") as f:
        f.write(html)

    print("HTML page saved")

    path = os.path.abspath(filename)

    webbrowser.open("file://" + path)

    print("Opened in browser")

if __name__ == "__main__":
    download_and_open()
```

## OUTPUT
<img width="1589" height="647" alt="{FFA61992-BDB0-4DBA-8E83-F4AE9070DC69}" src="https://github.com/user-attachments/assets/c144a70f-6f7a-4ab2-96e2-50b17b25857f" />

## Result
Thus the socket for HTTP for web page upload and download created and Executed
