# booked-docker

dockerfile for Booked Scheduler

## Usage

### Prepare
Download booked from official and put it, like below

```
├── booked-docker
│   ├── booked
```

```
cd booked
cp config/config.dist.php config/config.php
chmod 666 config/config.php
```

### Launch 

``` sh
docker-compose up -d
```

your booked will be hosted at 
http://localhost:80/Web/

### Config files

#### Booked

`booked/config/config.php`

#### Timezone (necessary for php)

`php/conf.d/timezone.ini`

#### Nginx

`conf.d/php.conf`
