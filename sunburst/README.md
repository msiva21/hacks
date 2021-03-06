## Suggested Usage

Pipe the output of some other tool or file, e.g.

```cat processes.txt | go run main.go```

or you can feed it a single process name on the command line:

```go run main.go someprocess```

You can also just output matches using the the ```-m``` flag:

``` cat processes.txt | go run main.go -m```

## Example Output

Note: output will be green if there is a match in the hardcoded process list.

```
14605870802367138151 : klifaa.sys
14076049386512171026 : cbk7.sys
6377259881933999545 : bhdrvx86.sys
18308913934889626123 : avgtpx86.sys
8144351048979905053 : bhdrvx64.sys
6976547106435497215 : avgtpx64.sys
15180155266747728342 : cyprotectdrv64.sys
13544031715334011032 : groundling64.sys
```

## Notes

Depends on the gookit/color package. Install first using:

```go get "github.com/gookit/color"```

You need to ensure you have `hardcoded_hashes.txt` in the same dir as this code. This code was written without care for production quality or error checking.

Thanks!

@cybercdh