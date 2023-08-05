# Installation
Clone this repository
```git clone git@bitbucket.org:clusteringteam/image-viewer.git```

Create a file containing images path
Go to images root directory
```find -type f > ../all_images_path.txt```

##Need to start two simple http server
- To host web view
- To host images

Choose any one of the following servers: Node JS(preferred) or python
(Apache or nginx web servers can also be used)

Use screens for nodeJS or python server
##HTTP Server
- Node js server ```http-server``` needs nodejs installed and http-server package installed. 
```http-server --port 8080```
```http-server --port 8081```
###Python server 
```python -m SimpleHTTPServer PORT_NUMBER```
```python -m SimpleHTTPServer 8080```
```python -m SimpleHTTPServer 8081```

The above two servers should be started as follows:
First in current repository directory for WebUI
Second in images directory to host images (Same path as the text file containing image paths)

Download all_images_path.txt to your local machine.
```scp -i /path/to/amazon/key user@IP:/path/to/all_images_path.txt ~/destination/in/local/machine```

Go to ```http://IP:PORT_NUMBER``` (IP address of the machine)

Select no of images to view in one page
Choose all_images_path.txt from your local machine
Click Load images