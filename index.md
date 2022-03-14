# PortScanner

[![Python](https://img.shields.io/badge/python-3.8-blue)](https://python.org)
![Level](https://img.shields.io/badge/Level-Easy-cyan)

Scan All Open Ports Of The Target IP.

A tool which is capable of scanning ports as `TCP` & `UDP` and detecting open and closed ones.


## Clone from GitHub
```bash
git clone https://github.com/MSFPT/PortScanner
```

## Example

<br>

|   argument    |      data       | utilization |
| ------------- | --------------- | ----------- |
| `--hostname` or `-h`  | hostname or ip | required |
| `--port` or `-p` | port | optional |
| `--minimum-port` or `-min-port` | minimum port | optional |
| `--maximum-port` or `-max-port` | maximum port | optional |
| `--protocol` | `TCP` / `UDP` | optional |
| `--filter` or `-f` | `all` / `open` / `closed` | optional |

<br>

### Types Run

<br>

```
python3 PortScanner --hostname github.com
```

```
python3 PortScanner -h github.com
```
**Usage:** Python3 PortScanner [hostname]

**Scan:** Port from 1 to 65535

**Protocol:** `TCP`

<br>

```
python3 PortScanner --hostname github.com --port 443
```

```
python3 PortScanner -h github.com -p 443
```

**Usage:** Python3 PortScanner [hostname] [port]

**Scan:** Port 443

**Protocol:** `TCP`

<br>

```
python3 PortScanner --hostname github.com --maximum-port 510
```

```
python3 PortScanner -h github.com -max-port 510
```

**Usage:** Python3 PortScanner [hostname] [max-port]

**Scan:** Port from 1 to 510

**Protocol:** `TCP`

<br>

```
python3 PortScanner --hostname github.com --minimum-port 80
```

```
python3 PortScanner -h github.com -min-port 80
```

**Usage:** Python3 PortScanner [hostname] [min-port]

**Scan:** Port from 80 to 65535

**Protocol:** `TCP`

<br>

```
python3 PortScanner --hostname github.com --minimum-port 80 --maximum-port 510
```

```
python3 PortScanner -h github.com -min-port 80 -max-port 510
```

**Usage:** Python3 PortScanner [hostname] [min-port] [max-port]

**Scan:** Port from 80 to 510

**Protocol:** `TCP`

<br>

```
python3 PortScanner --hostname github.com --port 6060 --protocol UDP
```

```
python3 PortScanner -h github.com -p 6060 --protocol UDP
```

**Usage:** Python3 PortScanner [hostname] [protocol]

**Scan:** Port 6060

**Protocol:** `UDP`

<br>

```
python3 PortScanner --hostname github.com --filter all
```

```
python3 PortScanner -h github.com -f all
```

**Usage:** Python3 PortScanner [hostname] [filter]

**Scan:** All Ports

**Protocol:** `TCP`

<br>

```
python3 PortScanner --hostname github.com --filter open
```

```
python3 PortScanner -h github.com -f open
```

**Usage:** Python3 PortScanner [hostname] [filter]

**Scan:** All Ports open

**Protocol:** `TCP`

<br>

```
python3 PortScanner --hostname github.com --filter closed
```

```
python3 PortScanner -h github.com -f closed
```

**Usage:** Python3 PortScanner [hostname] [filter]

**Scan:** All Ports closed

**Protocol:** `TCP`

<br><br>

### help
```
python3 PortScanner --help
```

```
python3 PortScanner -H
```

<br>

### developer
```
python3 PortScanner --developer
```

```
python3 PortScanner -D
```
