# State Managemnt
 <p>ASP.NET State management is a preserve state control and object in an application because ASP.NET web applications are stateless.</P>
  <p>A new instance of the Web page class is created each time the page is posted to the server. </p>
  <p>If a user enters information into a web application, that information would be lost in the round trip from the browser (MSDN).</p>
  
  # Type of State Management
 
 <p> 1. Server Side</P>
 
  <p>2. Client Side</p>
  
<p> There are two important objects which works on server side </p>
  <p> 1. Session </p>
  <p> 2. Application </p>
  <p> Session is a very important technique to maintain state. 
  Normally session is used to store information and identity. The server stores information using Sessionid.</p>
  
  <p> Application State is a server side management state. 
  It is also called application level state management. 
  In this mainly store user activity in server memory and application event shown in Global.asax file.</p>
  
  <p> Cookies are important on Client Side <p>
 
<p> Cookie is a small and an important part of ASP.NET. 
    In this store user information, session and application. 
    It can be created constant and temporary and they work with browser request. 
    Cookies are store on client side. The server can read cookies and abstract data.</p>
