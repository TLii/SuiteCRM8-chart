# SuiteCRM 8 Unofficial Chart
*SuiteCRM is a trademark of SalesAgility, Inc. This chart is unaffiliated with and not endorsed by SalesAgility.*
## General information
This chart deploys SuiteCRM version 8, licensed under AGPL v3. The chart can be deployed stand-alone, either with included internal or external database. 

The chart consists of a few containers. An NGINX container serves actual http(s) requests and "runs" the Angular frontend. The backend is built on top of Symfony, ie. php. The PHP is run in a PHP-FPM container. There is also an optional MariaDB container that can be enabled in values.yaml.

## License
This chart and SuiteCRM 8 are both licensed under AGPL version 3.

## Development
Pull requests are appreciated, although might not be accepted. The aim is to build a chart that can be deployed completely automatically, but other than that would be as vanilla as possible. The container image for SuiteCRM (more accurately, the php container) is built independently, see its [own repository](https://github.com/TLii/SuiteCRM8-docker).