# quantumdevice.github.io
the corp site of quantum device


how to deploy to vm
vm type : Ubuntu 16.04.1 LTS 

1. install docker on this vm      
   
   [Docker install steps for ubuntu](https://docs.docker.com/engine/installation/linux/ubuntu/)
         
2. use git clone to fetch the lastest code      
   ```javascript
   mkdir corpsite
   cd corpsite/
   git clone https://github.com/quantumdevice/quantumdevice.github.io.git
    
   ```

3. run docker      
    ```javascript
   sudo docker run -v /YOURWORKSPACE/corpsite/quantumdevice.github.io:/usr/share/nginx/html:ro -d -p 8081:80 --name website nginx
    ```
4. mapping the port to the loadblance 

