#RUN curl -o /tmp/backend.zip https://expense-builds.s3.us-east-1.amazonaws.com/expense-backend-v2.zip(backend files are copyed this link)

FROM node:20
# node js installation required 20 version
EXPOSE 8080
# just for info...backend port mensioned: 8080
ENV DB_HOST=mysql
#for database connection
RUN useradd expense
# add user : expense
RUN mkdir /opt/server 
#mkdir take anything /app or /opt/server
RUN chown expense:expense -R /opt/server
# create the access to this dir to expense user
WORKDIR /opt/server
# pwd path
COPY package.json .
COPY *.js .
# copy the pakage.json and .js files from our workspace
RUN npm install
# install npm
CMD [ "node","index.js" ]

# continously run node in index.js page(homepage)
