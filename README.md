# NiceStart

## Index

- ### [App's Design](#design)
  - #### [Design Colors](#colors)
  - #### [Component Styles](#styles)
- ### [App's Layouts](#layouts)
  - #### [Login page](#login)
  - #### [Signup page](#signup)
  - #### [Main page](#main)

## Design
NiceStart's design is focused on being simple and responsive, using a blue color palette
accented with black and white.

### Colors

> Note: color names are to reference the ones used in the code, they are not necessarily accurate.

- black <img src="https://placehold.co/15x15/000000/000000.png" alt="black icon"> `#000000`
- white <img src="https://placehold.co/15x15/FFFFFF/FFFFFF.png" alt="white icon"> `#FFFFFF`
- blue <img src="https://placehold.co/15x15/13678A/13678A.png" alt="blue icon"> `#13678A` -> mainly used for the gradient background
- emerald <img src="https://placehold.co/15x15/45C4B0/45C4B0.png" alt="emerald icon"> `#45C4B0` -> to draw user's attention where we want them to look at 
- transparent `#00FFFF00` -> to make the hollow effect, usually accompanied by a border

### Styles

Speaking of which, for the buttons there are two defined styles, ButtonFlat and ButtonOutlined:
- ButtonFlat
  - TextColor = black 
  - BackgroundColor = emerald
  - Stroke (border) = no
  - CornerRadius = 10dp
- ButtonOutlined
  - TextColor = white 
  - TextStyle = bold
  - BackgroundColor = transparent
  - Stroke (border) = yes, white
  - CornerRadius = 10dp

## Layouts
NiceStart is composed by 3 layouts: a login page, a signup page and a main page where the user will
be sent after completing one of the previous pages.
<br>
Every page has the app's logotype positioned on the top.

### Splash screen
> Note : see [activity_splash.xml](app/src/main/res/layout/activity_splash.xml)

Splash screen with tween logo animation and slogan to bring a warm welcome to the user.

<img src="videos/splash_screen_recording.gif"  alt="splash screen preview GIF" width="30%"/>

### Login
> Note : see [activity_login.xml](app/src/main/res/layout/activity_login.xml) / [activity_login.xml (land)](app/src/main/res/layout-land/activity_login.xml)

<br>
The login page has two inputs, one for the username and another for the password.
Under them there are positioned two buttons, which will allow the user to complete the login process
and switch to the signup page, respectively.  
<br><br>
  
<img src="images/login.png" alt="login page image" width="30%"/> <img src="images/login-land.png" alt="login land page image" width="60%"/>

### Signup

> Note : see [activity_signup.xml](app/src/main/res/layout/activity_signup.xml) / [activity_signup.xml (land)](app/src/main/res/layout-land/activity_signup.xml)

Our signup page is built quite simple, having only a username, email, password and password
confirmation input, all followed by a SIGNUP button that will complete the process and send the
user to the main page. On the other hand, there is a CANCEL button that will stop the process and
return the user to the login page.  
<br>
It also has an ActionBar that can do the same as the CANCEL button - returning to the login page -.  
<br>

<img src="images/signup.png" alt="signup page image" width="30%"/> <img src="images/signup-land.png" alt="signup land page image" width="60%"/>

### Main

> Note : see [activity_main.xml](app/src/main/res/layout/activity_main.xml)

After completing the login/signup process the user will be sent to the main page, which,
with a SwipeRefreshLayout, is able to reload an image in a WebView.<br><br>
Also has a menu on the ActionBar able to send the user to the profile page via MaterialAlertDialogBuilder.

<br>

<img src="images/main.png" alt="main page image" width="40%"/>
<img src="images/mainAlertDialog.png" alt="main page alert dialog image" width="40%"/>

### Profile
> Note : see [activity_profile.xml](app/src/main/res/layout/activity_profile.xml) / [activity_profile.xml (land)](app/src/main/res/layout-land/activity_profile.xml)

After the "Go to profile" option has been selected the user wil be sent to the profile page, which contains
a profile picture, the username and the bio/description the user
has.

<br>

<img src="images/profile.png" alt="profile page image" width="30%"/> <img src="images/profile-land.png" alt="profile land page image" width="60%"/>

> For this project I have used images of characters from Persona 3 Reload, which 
> are the intellectual property of ATLUS Co., Ltd., a division of SEGA Corporation. I fully acknowledge
> that these images, along with all other content related to Persona 3 Reload —including characters, designs,
> artwork, and any related media—are not my property and remain the exclusive rights of ATLUS.  
> <br>
> The use of these materials in my project is solely for illustrative purposes, and no ownership or 
> affiliation with ATLUS is implied.  
> <br>
> All rights reserved by ATLUS Co., Ltd.
