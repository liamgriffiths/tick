# tick

Runs the ["TICK stack"](https://www.influxdata.com/) in docker-compose.

## Running

```bash
$ cd latest/
$ docker-compose up
```

## Chronograph (visualization UI)

Open `localhost:8888`

## Send statsd metrics (demo)

```bash
$ while true; do echo -n "hello.count:$((RANDOM % 100))|c" | nc -w 1 -u 127.0.0.1 8125; done
```
