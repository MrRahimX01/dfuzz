
# dfuzz

Directory fuzzer for web applications




## Information


[![dfuzz Name](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)
[![1.0.0 Version](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)



## Common Switches

#### Normal Use

```http
  dfuzz -U https://example.com -W common.txt
```
#
#

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `-U` | `url` | provide the url |

#

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `-W`      | `wordlist` | path to  wordlist |

#

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `-o`      | `output` | path to save |

#

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `-fc`      | `filter code` | filter output with specific code |

#

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `-fs`      | `filter size` | filter output by specific response size |


#

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `--ext`      | `extesion` | append extension to the words |

#
#### Example

```http
  dfuzz -U https://example.com -W common.txt --ext php -fc 403 -fs 1981

```

## Installation

This is the compiled binary for amd 64

```bash
  git clone https://github.com/MrRahimX01/dfuzz
  cd dfuzz
  sudo cp dfuzz /bin
  dfuzz -h
```
    
