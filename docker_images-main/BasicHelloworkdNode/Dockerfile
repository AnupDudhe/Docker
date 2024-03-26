FROM node

LABEL Devops="Anup"

WORKDIR /usr/nodeapp

ADD .   .
#ADD https://github.com/AnupDudhe/nodejs-on-ec2.git  .

#WORKDIR nodejs-on-ec2 

EXPOSE 3000
RUN npm install 
CMD ["npm" , "start"]
