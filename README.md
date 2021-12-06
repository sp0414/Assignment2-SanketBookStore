# Assignment2-SanketBookStore 

Assignment 2

Program Name : SanketBookStore
Program Purpose : Create a MVC App 
Program Author : Sanketkumar Arvindbhai Patel
Program  Date :  2021-11-03


steps for the program : 


 Start the whole project again :: 

30/11/2021

9:30  and understand the question for assignment 

9:35 Create an asp.net web app
9:38 elect the Asp.net core model view controller
9:40 hange the startup.cs file
9:45 heck the public IActionResult interface
9:50 ckeck bugging
9:55 to Bootswatch.com and select the theme, I have selected Cyborg theme and download it and paste it to the local server. Also, Go to wwwroot and replace
   

10:38    the existing site.css file found in the main css folder and change file name bootstrap.min.css to bootstrap.css.
  Unfortunately, I got the error. the theme is not working on it properly.
10:40    Move forward to the next step, go to the _Layout.cshtml page the additional stylesheets and scripts from the CSS_JS.txt file
10:42    Change the nav-class from navbar-light to navbar dark and bg-white to bg-primary. Also, remove the text-dark from the nav bar.
10:43    add additonal Css and Js files which provide in the folder


5:35  Go to the _Layout.cshtml change the dropdown menu setting, add the code from the bootstrap files. Then, change the name of the dropdown to Content Management.
5:38   Got the error and stuck ......

01/12/2021

9:30     I got the error : Severity Code Description Project File Line Suppression State
9:38      Error CS0246 The type or namespace name 'ErrorViewModel' could not be found (are you missing a using directive or an assembly reference?) SanketBookStore C:\Users\W0776059\source\repos\SanketBookStore\SanketBookStore\SanketBookStore\Controllers\HomeController.cs  , Severity Code Description Project File Line Suppression State

10:00  ::  Error CS0433 The type 'IdentityUser' exists in both 'Identity.Stores, Version=1.2.7.0, Culture=neutral, PublicKeyToken=adb9793829ddae60' and 'Microsoft.Extensions.Identity.Stores, Version=5.0.0.0, Culture=neutral, PublicKeyToken=adb9793829ddae60' SanketBookStore C:\Users\W0776059\source\repos\SanketBookStore\SanketBookStore\SanketBookStore\Startup.cs 36 Active
10:30  :: Severity Code Description Project File Line Suppression State
Warning Unexpected comma after the last object member. SanketBookStore C:\Users\W0776059\source\repos\SanketBookStore\SanketBookStore\SanketBookStore\Properties\launchSettings.json 6
11:30  :: Got the error and could not run the app. the error is :
Severity Code Description Project File Line Suppression State
11:50  :: Error CS0433 The type 'IdentityUser' exists in both 'Identity.Stores, Version=1.2.7.0, Culture=neutral, PublicKeyToken=adb9793829ddae60' and 'Microsoft.Extensions.Identity.Stores, Version=5.0.0.0, Culture=neutral, PublicKeyToken=adb9793829ddae60' SanketBookStore C:\Users\W0776059\source\repos\SanketBookStore\SanketBookStore\SanketBookStore\Startup.cs 36 Active

12:20  ::   How i resolved: removed Identity.Store, made sure the Microsoft.Extensions.Identity.Stores was present in the project(s).
Conclusion - duplication resolved...


5:00 :: Got the Error ::
Message=An error occurred while creating the route with name 'default' and pattern '{area:Customer}{controller=Home}/{action=Index}/{id?}'.

5:30 Try to solve it but couldn't solved
6:15 Add the / in  pattern: "{area:Customer}/{controller=Home}/{action=Index}/{id?}"); and some change happen, the app is run but still got the error ..



