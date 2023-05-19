## commmand to clear our  admin first user:
docker-compose exec passbolt su -m -c "/usr/share/php/passbolt/bin/cake \
                                passbolt register_user \
                                -u name @gmail.com \
                                -f name  \
                                -l none \
                                -r admin" -s /bin/sh www-data
