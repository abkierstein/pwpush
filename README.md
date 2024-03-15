# pwpush
Command line Python password pusher via pwpush.com

If no password argument is given, a 20 character password comprised of letters, digits, and punctuation is generated.

### Usage:

```
usage: pwpush [-h] [-u URL] [-p PASSWORD] [-l LENGTH] [-d DAYS] [-v VIEWS]

Accept a password from stdin.

options:
  -h, --help            show this help message and exit
  -u URL, --url URL     Optional: Specify the URL of a local pwpush instance. ex: pwpush -u https://foobar.com
  -p PASSWORD, --password PASSWORD
                        Optional: User defined password.
  -l LENGTH, --length LENGTH
                        Optional: Length of auto-generated password. Ignored if password argument already provided.
  -d DAYS, --days DAYS  Optional: Specify the amount of days after which the password should expire.
  -v VIEWS, --views VIEWS
                        Optional: Specify the amount of views after which the password should expire.
```

ex.
```
> ./pwpush
Pass is: GKtPq:@%Q'r2Jakf7RQ0
URL: https://pwpush.com/p/tkfrluql1hi0f6qt

> ./pwpush -p foobar -u http://localhost:5100 -v 5
Pass is: foobar
URL: http://localhost:5100/p/630thim25imnm2x1

# -l is ignored since -p takes precedence
> ./pwpush -l 10 -p africanswallow
Pass is: africanswallow
URL: https://pwpush.com/p/zynqhemqkyvxi4q

> ./pwpush -l 10
Pass is: 0ezR.)cwg,
URL: https://pwpush.com/p/9ylhw57z4_qywugmqw
```
