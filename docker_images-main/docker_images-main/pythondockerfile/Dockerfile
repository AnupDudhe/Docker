FROM ubuntu:22.04
LABEL devops="anup dudhe"

USER root

RUN  apt update 
RUN  apt install git  python3 -y
RUN  apt install python3-pip -y 
RUN  pip3 install virtualenv   
RUN  virtualenv venv 
#RUN . /python-django/venv/bin/activate
RUN /bin/bash -c "source venv/bin/activate"
#RUN    source . venv/bin/activate 
RUN    apt update
    
RUN git clone https://github.com/mushfiq1998/string-tools-with-python-django.git
RUN    pip install Django 

WORKDIR python-django

#  RUN python manage.py makemigrations
#  RUN python manage.py migrate 
#  RUN python manage.py runserver
    
#RUN echo "from django.contrib.auth import get_user_model; User = get_user_model(); User.objects.create_superuser('admin', 'anupdudhe530@gmail.com', '12345678')" | python manage.py shell


EXPOSE  8000   
#CMD ["python3", "manage.py"]
#CMD ["sh", "-c", ". venv/bin/activate && python manage.py makemigrations && python manage.py migrate && python manage.py runserver 0.0.0.0:8000"]
#CMD ["sh", "-c", "source venv/bin/activate && python manage.py makemigrations && python manage.py migrate && python manage.py runserver 0.0.0.0:8000"]
#ENTRYPOINT ["python", "manage.py", "runserver", "0.0.0.0:8000"]
#ENTRYPOINT ["/bin/bash" ,"sh", "-c", ". venv/bin/activate && python manage.py makemigrations && python manage.py migrate && python manage.py runserver 0.0.0.0:8000"]
ENTRYPOINT ["sh", "-c", ". venv/bin/activate && python manage.py makemigrations && python manage.py migrate && python manage.py runserver 0.0.0.0:8000"]
#CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]  
#CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]  
#CMD /bin/bash