FROM arm64v8/nextcloud
MAINTAINER Khromium
ARG domain
RUN sed -i -e "s/\#ServerName www.example.com/ServerName ${domain}/g" /etc/apache2/sites-available/000-default.conf
# RUN sed -e "26i\    1 => '${domain}:80'" /var/www/html/config/config.php