# PHP-NGINX installer ansible playbook

This playbook will make redis up and running on remote server on port 6379.

## Installation

For installation you need to grab a fresh copy of app.

```bash

git clone https://github.com/ordidaad/ansible-redis.git

```

## Usage

```bash

ansible-playbook redis_installer.yml -i /path/to/your/inventory.cfg  -u root

```

## Test

After ansibe get his job done, your redis instance should be  ready and listening on port 6379.

```bash

redis-cli -a "YOUR-SECURE-PASSWORD"

127.0.0.1:6379> ping
PONG

```