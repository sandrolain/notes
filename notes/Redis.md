# Redis

## Resources
- [Redis Keyspace Notifications](https://redis.io/topics/notifications)
- [Redis notifications: Get key and value on expiration](https://stackoverflow.com/questions/18328058/redis-notifications-get-key-and-value-on-expiration)

## Commands

### Install Redis with homebrew

```sh
brew install redis
```

### Redis as homebrew service

```sh
brew services start redis
brew services list
```

### Configure Redis as homebrew service

```sh
mkdir /Users/sandrolain/redis-db
redis-cli
> CONFIG SET dir /Users/sandrolain/redis-db
```