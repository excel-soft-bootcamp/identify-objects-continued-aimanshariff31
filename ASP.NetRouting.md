# ASP.Net Routing
* Routing is the process of directing an HTTP request to a controller and the functionality of this processing is implemented in System.Web.Routing.
* MVC applications use the ASP.NET routing system, which decides how URLs map to controllers and actions.
### Example:

     public static void RegisterRoutes(RouteCollection routes)
      
      {
        
        routes.IgnoreRoute("{resource}.axd/{*pathInfo}");
			
         routes.MapRoute(
            "Process", "Process/{action}/{id}",
            defaults: new{
               controller = " Process", action = "List ", id =
               UrlParameter.Optional});
					
         routes.MapRoute(
            name: "Default", url: "{controller}/{action}/{id}",
            defaults: new{
               controller = "Home", action = "Index", id =
               UrlParameter.Optional});
      }
      
      
      
# Default Routing
* The default ASP.NET MVC project templates add a generic route that uses the following URL convention to break the URL for a given request into three named segments
* url: "{controller}/{action}/{id}"


This route pattern is registered via call to the MapRoute() extension method of RouteCollection.

// default Route

routes.MapRoute(

name: "Default",

url: "{controller}/{action}/{id}",

defaults: new { controller = "Home", action = "Index", id = UrlParameter.Optional }

routes.MapRoute(

name: "about",

url: "Home/About-WDI",

defaults: new { controller = "Home", action = "About", id = UrlParameter.Optional }

);

# Action Result

* Action Result is actually a data type. When it is used with action method, it is called return type
* As the name depicts these results are used for returning the content to the browser. There are 7 types of content returning results:

### View result
public ViewResult Index()  
{  
    return View();  
}  
      
 ### ContentResult
     public ContentResult content()
    {
        return Content(
        "<script> alert('Hi! I am from Mysore') </script>"
            );
    }
  
  ### RedirectionResult
    public RedirectResult content() { return Redirect("https://www.google.com"); }
   


