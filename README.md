# Passbolt Password Manager Demo Implementation

This repository contains a demo implementation for Passbolt Password Manager. Follow the instructions below to get started:

## Setup Instructions

1. Clone this repository by running the following command:

2. Copy the `env_template` file to `.env` and update all the required configurations in the `.env` file.

3. Modify the `traefik.yaml` file and add your email address to obtain a Let's Encrypt certificate for your domain.

4. Start the Passbolt containers by running the following command:
```
docker-compose up -d
```
5. Visit your domain to check if the Passbolt instance is running successfully.

6. To create an admin user, execute the following command:
```
docker-compose exec passbolt su -m -c "/usr/share/php/passbolt/bin/cake \
                             passbolt register_user \
                             -u <email address> \
                             -f <first name> \
                             -l <last name> \
                             -r admin" -s /bin/sh www-data
```


## Additional Resources

This serves as a good starting point for making further configuration changes. For more detailed guidance and assistance, please refer to the [Passbolt Help Center](https://help.passbolt.com/). The Help Center provides comprehensive documentation and support for Passbolt Password Manager.

Feel free to explore the features and functionalities of Passbolt Password Manager. Should you require any additional assistance, consult the Passbolt Help Center for further guidance.


