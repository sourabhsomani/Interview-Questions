# Introduction 
In this file you will get the Interview Question related to ASP.NET

## What is HTTP Handler?
The ASP.NET Web Forms model resolves an incoming request by dispatching the request to an HTTP handler component. According to the ASP.NET Web Forms model, the HTTP handler is expected to return HTML for the browser.

An HTTP handler component is an instance of a class that implements the **IHttpHandler** interface. 

```C#
public interface IHttpHandler
{
 public void ProcessRequest(HttpContext context);
 public bool IsReusable;
}
```

The name of the method ProcessRequest says it all about the intended semantics. It takes the context of the request as the input and ensures that the request is serviced. In the case of synchronous handlers, when ProcessRequest returns, the output is ready for forwarding
to the client. 

## Can HTTPHandlers be Async?
Yes, HTTP handlers can also work asynchronously according to the methods in the IHttpAsyncHandler interface.

## Every ASP.NET Page Inherits from which Class?
Every ASP.NET page class inherits from **System.Web.UI** class

## Which class inherits IHttpHandler?
In ASP.NET, the base page class is **System.Web.UI.Page** inherits IHTTPHandler Class.

## Describe The Page Controller pattern in ASP.NET Web Forms

![The Page Controller pattern in ASP.NET Web Forms](https://github.com/sourabhsomani/Interview-Questions/blob/master/ASP.NET/PageControllerpatternASPNET.png?raw=true)

