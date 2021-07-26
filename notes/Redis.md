# Redis

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