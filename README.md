# C-code-for-a-login-page-template
C# code for a login page template using ASP.NET framework




<%@ Page Language="C#" AutoEventWireup="true" CodeBehind="Login.aspx.cs" Inherits="YourNamespace.Login" %>

<!DOCTYPE html>

<html xmlns="http://www.w3.org/1999/xhtml">
<head runat="server">
    <title>Login Page</title>
    <link rel="stylesheet" href="style.css" />
</head>
<body>
    <form id="form1" runat="server">
        <div>
            <h1>Login</h1>
            <div>
                <label for="username">Username:</label>
                <asp:TextBox ID="username" runat="server"></asp:TextBox>
            </div>
            <div>
                <label for="password">Password:</label>
                <asp:TextBox ID="password" runat="server" TextMode="Password"></asp:TextBox>
            </div>
            <asp:Button ID="btnLogin" runat="server" Text="Login" OnClick="btnLogin_Click" />
        </div>
    </form>
</body>
</html>


using System;
using System.Collections.Generic;
using System.Linq;
using System.Web;
using System.Web.UI;
using System.Web.UI.WebControls;

namespace YourNamespace
{
    public partial class Login : System.Web.UI.Page
    {
        protected void Page_Load(object sender, EventArgs e)
        {
            // Code that runs when the page is loaded
        }

        protected void btnLogin_Click(object sender, EventArgs e)
        {
            string username = this.username.Text;
            string password = this.password.Text;

            // Perform login logic here

            Response.Redirect("Welcome.aspx");
        }
    }
}


MADE ENTIERLY BY ME ( CRYPTIC ). USE FOR UR FUTURE APP IDEAS, ENJOY!!!
