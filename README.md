# dirlstr

Finds Directory Listings or Open S3 Buckets from a list of URLs by traversing the URL paths, e.g.

```
  https://example.com/foo/bar/baz
  https://example.com/foo/bar/
  https://example.com/foo/
```

## Install

If you have Go installed and configured (i.e. with `$GOPATH/bin` in your `$PATH`):

```
go get -u github.com/cybercdh/dirlstr
```

## Usage

```
$ dirlstr <url>
```
or 
```
$ cat <file> | dirlstr
```

If a URL is found to expose a Directory Listing / open S3 Bucket, it will be printed to the console.

### Options

```
Usage of dirlstr:
  -c int
    	set the concurrency level (default 20)
  -t int
    	timeout (milliseconds) (default 10000)
  -v	Get more info on URL attempts
```

## Thanks
This code was heavily inspired by [@tomnomnom.](https://github.com/tomnomnom) 
In the immortal words of Russ Hanneman....."that guy f&ast;&ast;ks"
