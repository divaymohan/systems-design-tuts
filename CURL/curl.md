# CURL

An open source project that makes a command line tool and a library for transferring data using internet protocal.

## Simple command

```
 curl https://github.com/divaymohan
```

## With response header with header

```
curl --include http://localhost:5000/json-test
```

```
curl -i http://localhost:5000/json-test
```

## Post request with data

```
curl --data "data=divay&last=mohan" http://localhost:5000/methods
```

```
curl -d "data=divay&last=mohan" http://localhost:5000/methods
```

## Put request with data

```
curl -X PUT --data "data=divay&last=mohan" http://localhost:5000/methods
```

```
curl -X PUT -d "data=divay&last=mohan" http://localhost:5000/methods
```

## Delete request with data

```
curl -X DELETE http://localhost:5000/methods
```

## User name password

```
curl -u username:password http://localhost:5000/methods
```

## Download from curl

```
curl --output filename http://localhost:5000/methods
```

```
curl -o filename http://localhost:5000/methods
```

## To see json response in json format

```
curl http://localhost:5000/methods/json | jq
```

## To get only response header

```
curl -I http://localhost:5000/methods
```

## To follow the redirect and print both the headers

```
curl -I -L http://localhost:5000/redirect
```

