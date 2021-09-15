# HTMLHelpers #

* The HtmlHelper class renders HTML controls in the razor view. 
* It binds the model object to HTML controls to display the value of model properties into those controls and also assigns the value of the controls to the model properties while submitting a web form.
* So always use the HtmlHelper class in razor view instead of writing HTML tags manually.
![image](https://user-images.githubusercontent.com/86050998/133398904-df68b389-d45c-49a1-8327-55cd024b16f8.png)


* In the above figure, @Html is an object of the HtmlHelper class. 
 * Html is a property of the HtmlHelper class included in base class of razor view WebViewPage. 
 * The ActionLink() and DisplayNameFor() are extension methods included in the HtmlHelper class.


### HTMLHelper Methods ###
The fllowing lists the HtmlHelper methods .




1.Html.ActionLink()

2.Html.TextBox()

3.Html.TextArea()

4.Html.CheckBox()

5.Html.RadioButton()

6.Html.DropDownList()

7.Html.ListBox()

8.Html.Password()
  
9.Html.Display()

10.Html.Label()
