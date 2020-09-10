---
layout: post
title:  "ASP.NET HTTP Modules and HTTP Handlers!"
date:   2020-09-11 23:42:47 +0530
categories: jekyll update
---
Summary

HTTP modules and HTTP handlers are an integral part of the ASP.NET architecture. While a request is being processed, each request is processed by multiple HTTP modules (for example, the authentication module and the session module) and is then processed by a single HTTP handler. After the handler has processed the request, the request flows back through the HTTP modules

HTTP modules overview
Modules are called before and after the handler executes. Modules enable developers to intercept, participate in, or modify each individual request. Modules implement the IHttpModule interface, which is located in the System.Web namespace.

Events:

1. BeginRequest
2. AuthentcateREquest
3. AuthorizeRequest
4. ResolveRequestCache
5. AcquireRequestState
6. PreRequestHandlerExecute
7. PostRequestHandlerExecute
8. ReleaseRequestState
9. UpdateRequestCache
10. EndRequest


Source: https://docs.microsoft.com/en-us/troubleshoot/aspnet/http-modules-handlers
