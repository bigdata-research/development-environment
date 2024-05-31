How to install Oracle 19.3.

Can see reference github : https://github.com/steveswinsburg/oracle19c-docker

- Download file 'LINUX.X64_193000_db_home.zip' in this link : https://www.oracle.com/id/database/technologies/oracle19c-linux-downloads.html.
puth in folder : ./dockerfiles/19.3.0

- Build Image Oracle : ./buildContainerImage.sh -e -v 19.3.0 -p

- docker compose up -d

If you have trouble when creating image, please see documentation : https://github.com/oracle/docker-images.git

