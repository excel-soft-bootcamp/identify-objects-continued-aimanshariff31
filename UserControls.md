# User Controls
* ASP.NET allows the users to create controls
 ### The user defined controls are categorized into:
 1. User Controls
 2. Custom Controls
  #### User Controls
 * These are derived from the System.Web.UI.UserControl class.
 * They have an .ascx extension.
 * They may not contain any , , or tags.
 * They have a Control directive instead of a Page directive.

#### Custom Controls
* They are compiled into a Dynamic Link Library (DLL)
* They can be created in other following ways
1. By deriving a custom control from an existing control
2. By composing a new custom control combing two or more existing controls.
3. By deriving from the base control class
