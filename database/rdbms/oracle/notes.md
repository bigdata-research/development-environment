### How to install Oracle 19.3 in docker

- Download file 'LINUX.X64_193000_db_home.zip' in this link : https://www.oracle.com/id/database/technologies/oracle19c-linux-downloads.html. put in folder ./dockerfiles/<version_database>/*.zip

- build image : ./buildContainerImage.sh -e -v 19.3.0 -p

If you have trouble when creating image, please see documentation : https://github.com/oracle/docker-images.git

