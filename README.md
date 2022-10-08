# wordpress-fio-test
A repository to run a simple wordpress container


Step to run :
- Download this repo
- If using downloaded as ZIP, unzip the file :
  
  $ unzip main
  
- Change directory to wordpress-fio-test-main :
  
  $ cd wordpress-fio-test-main
  
- Build the image :
  
  $ podman build -t fio-wordpress .
  
- Run the container :
  
  $ podman run --name fio-wordpress -p 8080:80 -d fio-wordpress
  
- Check the container status :
  
  $ podman ps
  
- Access the wordpress :
  - Using curl :
  
    $ curl <YOUR_MACHINE_IP_ADDRESS>:8080/test.html
    
  - Using web browser :
      Access the web on your favorite web browser to -> <YOUR_MACHINE_IP_ADDRESS>:8080/test.html
 
 It should result like this :
 FIO DOCKER WORDPRESS ASSESSMENT TEST
