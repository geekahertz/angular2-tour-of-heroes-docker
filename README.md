# angular2-tour-of-heroes

Docker container for creating a dev enviroment for learning Angular2: John Papa's Tour of Heros Demo

# How to use this image

## Running container

    sudo docker run -it -p 139:139 -p 445:445 -p 8000:8000 -p 3001:3001 \
        -dman1680/angular2-tour-of-heroes samba.sh \
        -u "testuser;pass" -s "usr;/usr;no;no;no;testuser"
        
## Accessing container files
    
    TODO

