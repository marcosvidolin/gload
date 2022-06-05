# gload
A very simple load test tool

## Usage

```shell
gload -s senarios.yml
```

## Scenario file example

```yaml
CreateUser:
  url: https://api.gloadsys.com/users
  mehotd: POST
  timeout: 5
  headers:
    Content-Type: application/json
  body: |
    {
      "username": "gloaduser",
      "email": "gload@mail.com"
    }

GetAllGroups:
  url: https://api.gloadsys.com/groups
  mehotd: GET
  timeout: 5
  headers:
    Content-Type: application/json
```