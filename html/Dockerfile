FROM nginx

COPY ./ /usr/share/nginx/html


RUN mkdir /etc/nginx/templates
COPY ./default.conf.template /etc/nginx/templates/
# WORKDIR /etc/nginx/conf.d/
# COPY html/default.conf default.conf

EXPOSE 8080