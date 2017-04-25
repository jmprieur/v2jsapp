---
services: active-directory
platforms: javascript
author: jmprieur
---

# Sign in Azure AD + MSA Users using Javascript Open Source Library

This simple sample demonstrates how to use the Microsoft Graph to send an email after being authenticated with msal.js. (doing oAuth 2.0 against the AAD v2.0 endpoint). It does not require any Single Page Application Framework.

## Steps to Run

1. Register your Azure AD v2.0 app. 
    - Navigate to the [App Registration Portal](https://identity.microsoft.com). 
    - Go to the the `My Apps` page, click `Add an App`, and name your app.  
    - Set a platform by clicking `Add Platform`, select `Web`, and add a Redirect URI of ```http://localhost:8000/```.

2. Clone the code.
  ```
  git clone https://github.com/jmprieur/v2jsapp.git
  ```

3. Inside index.html, set your application/client id from the App Registration Portal. 

4. Run the web app for port 8000, and navigate to http://localhost:8000. If you have Python installed you can run the following command, 

  ```
  python -m SimpleHTTPServer 8000
  ```

## Questions and Issues

Please file any questions or problems with the sample as a github issue.  You can also post on StackOverflow with the tag ```azure-active-directory```.  For oAuth2.0 library issues, please see note above. 

This sample was with Google Chrome version 57.0 and Edge on Windows 10.

## Acknowledgements

This sample was adapted from the hello.js sample: https://github.com/Azure-Samples/active-directory-javascript-graphapi-web-v2
