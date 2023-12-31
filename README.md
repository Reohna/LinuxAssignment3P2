Simple Server with Load Balancer

The included backend server runs on port 8080, 127.0.0.1:8080

## Included material

- backend binary, hello-server
- frontend, index.html
- nginx configuration file, hello.conf
- service file for backend, hello-server.service
- config for setting up servers, cloud-config.yml
- example curl commands for testing your server, curl.md

## Where to place files

### Where to store the index.html

```
/var/www/my-sites/index.html
```

### Where to store the hello-server.service file

```
/etc/systemd/system/hello-server.service
```

### Where to store the hello.conf file

```
/etc/nginx/sites-available/hello.conf
```

### Create a symbolic link to the hello.conf file

Move to the folder:
   ```
   cd /etc/nginx/sites-enabled
   ```
Create symbolic link to the hello.conf file:
   ```
   ln -s /etc/nginx/sites-available/hello.conf
   ```

### Where to store the server to work with my configurations:

```
/home/web/hello-server
```

Please create this directory ```/var/log/hello-server/``` for your backend.log to store logs. 
