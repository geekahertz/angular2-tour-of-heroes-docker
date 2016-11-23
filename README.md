# angular2-tour-of-heroes

Samba docker container for learning Angular2: John Papa's Tour of Heros Demo

# How to use this image
## Host setup
- Docker toolbox for Windows v1.12.2
- Oracle VM VirtualBox 5.1.6

## Running container

    sudo docker run -it -p 139:139 -p 445:445 -p 8000:8000 -p 3001:3001 -d dman1680/angular2-tour-of-heroes samba.sh -u "testuser;pass" -s "usr;/usr;no;no;no;testuser"
        
## Accessing container files

Find docker machine's ip

    docker-machine ip

Access network share folder
    
    //<docker machine's ip>/usr
    # login: testuser / pass
