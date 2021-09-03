# AJAX
* AJAX stands for Asynchronous JavaScript and XML.
* This is a cross platform technology which speeds up response time.
* The AJAX server controls add script to the page which is executed and processed by the browser.
* The control toolbox in the Visual Studio IDE contains a group of controls called the 'AJAX Extensions':-
#### Among them are:-
1. Update panel control
2. Script manager control

## Update Panel Control
* The UpdatePanel control is a container control and derives from the Control class.
* It acts as a container for the child controls within it and does not have its own interface.
* When a control inside it triggers a post back, the UpdatePanel intervenes to initiate the post asynchronously and update just that portion of the page.
##### Syntax:-
string time = DateTime.Now.ToLongTimeString();
lblpartial.Text = "Showing time from panel" + time;
lbltotal.Text = "Showing time from outside" + time;

## The ScriptManager Control
* The ScriptManager control  must be present on the page for other controls to work.
##### Syntax:-
<asp:ScriptManager ID="ScriptManager1" runat="server">
</asp:ScriptManager>
