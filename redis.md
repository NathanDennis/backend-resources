## Resources and reference material for Redis

### YouTube videos / series

- [Installing Redis on Windows](https://www.youtube.com/watch?v=ncFhlv-gBXQ) - Raghav Pal

### Playgrounds

- [Try Redis](https://try.redis.io/) - try.redis.io

### Commands

#### SET - `SET key value` - Set a key value pair

 - Example: `SET name "Nathan"`

#### GET - `GET key` - Get the value of a specified key

 - Example: `GET name` // Returns "Nathan"


#### EXISTS - `EXISTS key` - Check if a specific key exists in the DB

 - Example: `EXISTS name`


#### DEL - `DEL key` - Delete a specific key and it's value from the DB

 - Example: `DEL name` // Deletes the key 'name' and it's associated value


#### EXIPRE - `EXPIRE key time` - Set a specific key to expire after a specified time value

 - Example: `EXPIRE session 10` - Set the key 'session' to expire after 10 seconds
