
# dfuzz

Directory fuzzer for web applications






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
    
