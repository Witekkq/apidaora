# dataclassesapi

<p align="center" style="margin: 3em">
  <a href="https://github.com/dutradda/dataclassesapi">
    <img src="https://dutradda.github.io/dataclassesapi/dataclassesapi.svg" alt="dataclassesapi" width="300"/>
  </a>
</p>

<p align="center">
    <em>Asgi App using typing annotation</b></em>
</p>

---

**Documentation**: <a href="https://dutradda.github.io/dataclassesapi" target="_blank">https://dutradda.github.io/dataclassesapi</a>

**Source Code**: <a href="https://github.com/dutradda/dataclassesapi" target="_blank">https://github.com/dutradda/dataclassesapi</a>

---


## Key Features

- Declare request object as @dataclass:
    + `PathArgs` for values on path
    + `Query` for values on query string
    + `Headers` for values on headers
    + `Body` for values on body

- Declare response object as @dataclass:
    + `Headers` for values on headers
    + `Body` for values on body


## Requirements

 - Python 3.7+
 - [dataclassesjson](https://github.com/dutradda/dataclassesjson) for json validation/parsing
 - [orjson](https://github.com/ijl/orjson) for json/bytes serialization


## Instalation
```
$ pip install dataclassesapi
```


## Basic example

```python
{!./src/index/index_00_basic.py!}
```

Running the server (needs uvicorn [installed](https://www.uvicorn.org)):

```bash
{!./src/index/index__server.bash!}
```

```
{!./src/index/index__server.bash.output!}
```

Quering the server (needs curl [installed](https://curl.haxx.se/docs/install.html)):

```bash
{!./src/index/index_00_basic_curl.bash!}
```

```
{!./src/index/index_00_basic_curl.bash.output!}
```


## Example for complete request/response

```python
{!./src/index/index_01_complete.py!}
```

Running the server:

```bash
{!./src/index/index__server.bash!}
```

```
{!./src/index/index__server.bash.output!}
```

Quering the server:

```bash
{!./src/index/index_01_complete_curl.bash!}
```

```
{!./src/index/index_01_complete_curl.bash.output!}
```