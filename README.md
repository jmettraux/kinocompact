
# kinocompact

A script to compact [asciinema](https://asciinema.org) JSON files.

Sets a max wait time (like `asciinema -w 1.2` does, granted), and compacts backspaces (blunders are "compacted" out).

```
$ kinocompact -h
Usage: kinocompact [options] [filename or -]
    -t, --type-speed SECONDS         Sets the type speed, defaults to 0.077
    -w, --wait-speed SECONDS         Sets the max wait speed, defaults to 1.0
        --stdin                      Reads incoming asciinema json file on stdin
    -o, --out-file FILENAME          Sets the output file, defaults to STDOUT
    -B, --no-backspace-compaction    Disable backspace compaction
    -h, --help                       Print this help
```

```
$ kinocompact a.json > b.json
```

## license

MIT, see [LICENSE.txt](LICENSE.txt)

