
# kinocompact

```
> "There's a lighthouse in the middle of Prussia
>  A white house in a red square
>  I'm living in films for the sake of Russia
>  A Kino Runner for the DDR"
>     Sisters of Mercy - Dominion / Mother Russia
```

A script to compact [asciinema](https://asciinema.org) JSON files.

Sets a max wait time (like `asciinema -w 1.2` does, granted), and compacts backspaces (blunders are "compacted" out).

Unfortunately, cannot compact blunders made inside of Vi\[m\].

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

