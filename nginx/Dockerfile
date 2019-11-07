FROM nginx

MAINTAINER NGUYEN VAN HUONG<nguyenhuong791123@gmail.com>

RUN \
apt-get update && \
apt-get install unzip wget -y && \
rm -rf /var/lib/apt/lists/*
#ADD www /var/www
#ADD nginx.conf:/etc/nginx/nginx.conf
# RUN mkdir /etc/nginx/tls
#ADD ./tls/sc.crt /etc/nginx/sc.crt
#ADD ./tls/sc.key /etc/nginx/sc.key

RUN mkdir /root/logs
RUN chmod 755 -R /root
#RUN chmod 400 /etc/nginx/sc.key

EXPOSE 80
CMD [ "nginx", "-g", "daemon off;" ]
