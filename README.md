# Microsoft SQL server docker compose

My personal docker compose for standalone MS-SQL 2019. Uses the official MS SQL 2019 image from docker hub.

## Requirements
* Docker
* Docker composer

## Usage
* Clone repository (`git clone https://github.com/coderkoala/docker-compose-mssql`)
* Initalize your `docker-compose.yml` file : `cp docker-compose.example.yml docker-compose.yml`
* Configure password in `docker-compose.yml` file.
* Start the container (`docker-compose up -d`)

To stop the container, use the `docker-compose stop` command.

## Connecting

By default, if it is self-hosted, all you need to do is connect through the pegged localhost alias. Depending on your system:

* 127.0.0.1,1433
* 0.0.0.0,1433

Credentials will be `sa`:`YOUR_STRONG_PASSWORD_HERE_123` by default.

## Notes

Note that unless if you adhere to MSSQL's security policy for passwords, your initialization of the container WILL fail.

## Ports

The default exposed port is on 1433, same as a default MSSQL instance.

## License
This project is released under the GNU GPL-3.0 license. Check out the [LICENSE](LICENSE) file for more information.
