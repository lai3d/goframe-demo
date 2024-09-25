# GoFrame Template For SingleRepo

Quick Start: 
- https://goframe.org/pages/viewpage.action?pageId=1114399

Use this to build docker image

```bash
gf docker -tn go-frame-demo:v0.0.2
```

Run using docker compose

```bash
✗ docker compose up
[+] Running 1/0
 ✔ Container go-frame-demo  Recreated                                                                                                                                                                                                                                          0.0s 
Attaching to go-frame-demo
go-frame-demo  | 2024-09-25 08:25:17.194 [INFO] {d2bf61e5316ff817d3a9bc3227f34e99} swagger ui is serving at address: http://127.0.0.1:8000/swagger/
go-frame-demo  | 2024-09-25 08:25:17.194 [INFO] pid[1]: http server started listening on [:8000]
go-frame-demo  | 2024-09-25 08:25:17.194 [INFO] {d2bf61e5316ff817d3a9bc3227f34e99} openapi specification is serving at address: http://127.0.0.1:8000/api.json
go-frame-demo  | 
go-frame-demo  |   ADDRESS | METHOD |   ROUTE    |                           HANDLER                            |           MIDDLEWARE             
go-frame-demo  | ----------|--------|------------|--------------------------------------------------------------|----------------------------------
go-frame-demo  |   :8000   | ALL    | /api.json  | github.com/gogf/gf/v2/net/ghttp.(*Server).openapiSpec        |                                  
go-frame-demo  | ----------|--------|------------|--------------------------------------------------------------|----------------------------------
go-frame-demo  |   :8000   | GET    | /hello     | goframe-demo/internal/controller/hello.(*ControllerV1).Hello | ghttp.MiddlewareHandlerResponse  
go-frame-demo  | ----------|--------|------------|--------------------------------------------------------------|----------------------------------
go-frame-demo  |   :8000   | ALL    | /swagger/* | github.com/gogf/gf/v2/net/ghttp.(*Server).swaggerUI          | HOOK_BEFORE_SERVE                
go-frame-demo  | ----------|--------|------------|--------------------------------------------------------------|----------------------------------
go-frame-demo  | 
```

## Access

http://localhost:8080/hello

