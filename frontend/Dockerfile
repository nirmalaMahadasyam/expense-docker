FROM nginx
# install nginx
RUN rm -rf /usr/share/nginx/html/index.html
# default index nginx homepage we don't want.
RUN rm -rf /etc/nginx/nginx.conf
RUN rm -rf /etc/nginx/conf.d/default.conf

# nginx.conf,default.conf to remove and keep our own conf file: expense.conf
COPY expense.conf /etc/nginx/nginx.conf
# expense.conf to add nginx home path
COPY code /usr/share/nginx/html/
# code(folder) in our workspace this files contains images,css etc... these all copy to path:/usr/share/nginx/html/
