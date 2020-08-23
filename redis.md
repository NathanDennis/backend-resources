## Resources and reference material for Redis

### YouTube videos / series

- [Installing Redis on Windows](https://www.youtube.com/watch?v=ncFhlv-gBXQ) - Raghav Pal

### Playgrounds

- [Try Redis](https://try.redis.io/) - try.redis.io

### Basic Commands

#### SET - `SET key value` - Set a key value pair

 - Example: `SET name "Nathan"`

#### GET - `GET key` - Get the value of a specified key

 - Example: `GET name` - Returns "Nathan"

#### MSET - `MSET key value key value...` - Set multiple key value pairs

 - Example: `MSET a 1 b 2 c 3` 
 
#### MGET - `MGET key key...`

 - Example: `MGET a b c` - returns "1" "2" "3"

#### EXISTS - `EXISTS key` - Check if a specific key exists in the DB

 - Example: `EXISTS name`


#### DEL - `DEL key` - Delete a specific key and it's value from the DB

 - Example: `DEL name` - Deletes the key 'name' and it's associated value


#### EXIPRE - `EXPIRE key time` - Set a specific key to expire after a specified time value

 - Example: `EXPIRE session 10` - Set the key 'session' to expire after 10 seconds

#### INCRBY - `INCRBY key number` - Increment a key's value by a set amount

 - Example: `INCRBY count 20` - Increments the value of `count` by 20
 
#### DECRBY - `DECRBY key number` - Decrement a key's value by a set amount

 - Can also use DECR to decrement by a default value of 1 
 - Example: `DECRBY count 10` - Decrement the value of `count` by 10
 
___

### Hashes
Stores field values on a key similar to JavaSript Objects

#### HMSET - `HMSET eky field value`

 - Example: `HMSET user id 45 name "Nathan"` - Creates a hash called `user` with fields named `id` and `name` with their specified values
 
#### HMGET - `HMGET key field` - Gets the value of a specified field on the required key

 - Example: `HMGET user id` - Returns "45"
 
#### HGETALL - `HGETALL key` - Gets all the field value pairs from a specified key

 - Example: `HGET ALL user` - Returns "id" "45" "name" "Nathan"
 
___

