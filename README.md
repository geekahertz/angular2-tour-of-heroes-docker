# angular2-tour-of-heroes

Samba docker container for learning Angular2: John Papa's Tour of Heros Demo

# How to use this image
## Host setup
- Docker toolbox for Windows v1.12.2
- Oracle VM VirtualBox 5.1.6 
or 
- Hyper-V (see https://msdn.microsoft.com/en-us/virtualization/hyperv_on_windows/quick_start/walkthrough_install)

## Running container

    docker run -p 139:139 -p 445:445 -p 8000:8000 -p 3001:3001 -d dman1680/angular2-tour-of-heroes
        
## Accessing container
### Find docker machine ip

    docker-machine ip

### Find container id

    docker ps

### Browse demo webpage
    
    http://<docker machine ip>:8000

### Setup network share access

    docker exec -d <container id> samba.sh -u "testuser;pass" -s "usr;/usr;no;no;no;testuser"

### Access network share folder
    
    \\<docker machine ip>\usr
    # login: testuser / pass

### Enter container's bash
    
    docker exec -it <container id> bash
