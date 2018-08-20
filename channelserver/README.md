# Simple websocket pairsona server

## Config options:

Options can be set as ENV vars (prefixed with "`PAIR_`", e.g.
"`PAIR_PORT="8000"`"), or as arguments ("`--port=8000`").

See `src/settings.rs` for defaults.

## GeoIP lookup

This will require a [maxmind GeoIP](https://dev.maxmind.com/geoip/geoip2/geolite2/) lookup database. This presumes that
the database will be in `mmdb/latest/GeoLite2-City.mmdb`. Use the 
`mmdb_loc` to specify a different path (*Note:* if running in the debugger,
you may need to create a symlink under `target/debug`.) 

## Compile and run:

After installing rust via [rustup](https://rustup.rs/):

```sh
$ cargo run
```

