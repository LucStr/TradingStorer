# Trading Storer

This application is used to store up to date Trading Information inside a [TimescaleDB](https://www.timescale.com/).

# Requirements
- docker
- docker-compose

# Installation
1. `cp .env.example .env`
2. Adjust Settings in .env file.
3. run `docker-compose up -d`
4. locate Adminer within your browser and use your credentials configured in .env to login. Note the server is 'db'
5. Add Your Trackers within Adminer. A Tracker consists of a Trading Pair and an Exchange.
6. Restart the app container: `docker-compose restart app`.

# Database
The Database uses the following schema: 
![image](https://user-images.githubusercontent.com/25279790/196005994-177504dc-4f1d-4c65-b688-329d5e7d81bf.png)

