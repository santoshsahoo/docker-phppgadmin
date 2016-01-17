# docker-phppgadmin
phpPgAdmin Docker image.


docker run -d --restart=always --name phppgadmin --hostname phppgadmin -e SET_REAL_IP_FROM=172.17.0.0/16 -e ADMINADDR=root@cloyne.org -e REMOTES=mail.cloyne.net -v /srv/var/hosts:/etc/hosts:ro -v /srv/var/log/phppgadmin:/var/log/nginx cloyne/phppgadmin
