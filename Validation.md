# Validation Controls In ASP.NET
* Validation is important part of any web application
* An important aspect of creating ASP.NET Web pages for user input is to check that the information users enter is valid.
* ASP.NET provides a set of validation controls that provide an easy-to-use but powerful way to check for errors and, if necessary, display messages to the user.

## There are six types of validation controls in ASP.NET
* RequiredFieldValidation Control
* CompareValidator Control
* RangeValidator Control
* RegularExpressionValidator Control
* CustomValidator Control
* ValidationSummary

1. RequiredFieldValidator:-The RequiredFieldValidator control ensures that the required field is not empty. It is generally tied to a text box to force input into the text box.
#### Syntax:-
<asp:RequiredFieldValidator ID="rfvcandidate" runat="server" ControlToValidate ="ddlcandidate" ErrorMessage="Please choose a candidate" InitialValue="Please choose a candidate">
</asp:RequiredFieldValidator>

2. RangeValidator Control:-The RangeValidator control verifies that the input value falls within a predetermined range. It has three specific properties: Type, MinimumValue, MaximumValue.
#### Syntax:-
<asp:RangeValidator ID="rvclass" runat="server" ControlToValidate="txtclass" ErrorMessage="Enter your class (6 - 12)" MaximumValue="12" MinimumValue="6" Type="Integer">
</asp:RangeValidator>

3. CompareValidator Control:-The CompareValidator control compares a value in one control with a fixed value or a value in another control. It has the following specific properties: Type, ControlToCompare, ValueToCompare, Operator.
#### Syntax:-
<asp:CompareValidator ID="CompareValidator1" runat="server" ErrorMessage="CompareValidator">
</asp:CompareValidator>

4. Regular Expression Validator:-Ensures that the value of an input control matches a specified pattern
#### Syntax:-
<asp:RegularExpressionValidator ID="string" runat="server" ErrorMessage="string" ValidationExpression="string" ValidationGroup="string">
</asp:RegularExpressionValidator>

5. CustomValidator:- The CustomValidator control allows writing application specific custom validation routines for both the client side and the server side validation.
#### Syntax:-
<asp:CustomValidator ID="CustomValidator1" runat="server"
ClientValidationFunction=.cvf_func. ErrorMessage="CustomValidator">
</asp:CustomValidator>

6. ValidationSummary:-The ValidationSummary control does not perform any validation but shows a summary of all errors in the page. The summary displays the values of the ErrorMessage property of all validation controls that failed validation.
#### Syntax:-
<asp:ValidationSummary ID="ValidationSummary1" runat="server"
DisplayMode = "BulletList" ShowSummary = "true" HeaderText="Errors:" />
