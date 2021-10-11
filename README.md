# pwpush
Command line Python password pusher via pwpush.com

If no password argument is given, a 20 character password comprised of letters, digits, and punctuation is generated.

### Usage:

```
usage: pwpush [-h] [-u URL] [-p PASSWORD]

Accept a password from stdin.

optional arguments:
  -h, --help            show this help message and exit
  -u URL, --url URL     Optional: Specify the URL of a local pwpush instance. ex: pwpush -u https://foobar.com
  -p PASSWORD, --password PASSWORD
                        Optional: User defined password.
```

ex.
```
> ./pwpush
Pass is: GKtPq:@%Q'r2Jakf7RQ0
URL: https://pwpush.com/p/tkfrluql1hi0f6qt

> ./pwpush -p foobar -u http://localhost:5100`
Pass is: foobar
URL: http://localhost:5100/p/630thim25imnm2x1
```
