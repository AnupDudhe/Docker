FROM mysql:latest

LABEL database="studentapp"

ENV MYSQL_ROOT_PASSWORD=1234

COPY student.sql /docker-entrypoint-initdb.d/

CMD /bin/bash

# although container is running with above file ,
#but while taking access it giving few errors to work with container.
#so run bottom docker file
#and once container is up
#hit docker exec -it containerid bash
#then once your inside container
#hit mysql -p1234
#your mysql will openup

# FROM mysql:latest

# LABEL database="studentapp"

# ENV MYSQL_ROOT_PASSWORD=1234

# COPY student.sql /docker-entrypoint-initdb.d/

