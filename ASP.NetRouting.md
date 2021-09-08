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
   
   


