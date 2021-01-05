# Setup
You can find the package, [here](https://pypi.org/project/redis-persistence/).
```
pip3 install redis-persistence
```

# Requirements
* Python 3.8
* Redis 3.5

# Import
```python
from redispersistence.persistence import RedisPersistence
```

# Usage
You need to use this persistence with [pyton-telegram-bot](https://github.com/python-telegram-bot/python-telegram-bot) module.
```python
redis_instance = Redis(host='localhost', port=6379, db=0)
persistence = RedisPersistence(redis_instance)
updater = Updater(BOT_TOKEN, persistence=persistence)
```