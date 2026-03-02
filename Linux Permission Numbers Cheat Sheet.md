
## The Three Digits: `[Owner] [Group] [Others]`

Each digit is the **sum** of:

|Value|Permission|
|---|---|
|4|Read (r)|
|2|Write (w)|
|1|Execute (x)|
|0|None (-)|

---

## Common Permission Numbers

|Octal|Symbolic|Meaning|
|---|---|---|
|777|rwxrwxrwx|Full access for everyone|
|755|rwxr-xr-x|Owner full, others read/execute|
|700|rwx------|Owner full, others nothing|
|644|rw-r--r--|Owner read/write, others read|
|640|rw-r-----|Owner read/write, group read|
|600|rw-------|Owner read/write only|
|400|r--------|Owner read only|
|000|----------|No permissions for anyone|

---

## Single Digit Breakdown

|Digit|r|w|x|Symbolic|
|---|---|---|---|---|
|7|✓|✓|✓|rwx|
|6|✓|✓|✗|rw-|
|5|✓|✗|✓|r-x|
|4|✓|✗|✗|r--|
|3|✗|✓|✓|-wx|
|2|✗|✓|✗|-w-|
|1|✗|✗|✓|--x|
|0|✗|✗|✗|---|

---

## Usage

```bash
chmod 755 file.sh      # Set permissions
chmod +x file.sh       # Add execute for all
chmod u+w file.txt     # Add write for owner
ls -l file.txt         # View permissions
```

---

## Special Bits (4th digit prefix)

|Octal|Name|Effect|
|---|---|---|
|4xxx|Setuid|File runs as owner (e.g. `4755`)|
|2xxx|Setgid|File runs as group / inherit group dir|
|1xxx|Sticky bit|Only owner can delete file in dir|

> **Example:** `chmod 1777 /tmp` — anyone can write, only owner can delete their files.