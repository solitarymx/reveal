# reveal
Ionic ion-input reveal issue

Create new ionic/angular project (tabs) and I placed 2 inputs for username and password. I typed my username incomplete and started typing my password.
When I realized this, I left my password halfway and corrected my username. Then I wanted to type my password again, but the "eye" icon does not appear again.

1 - dom = < div pseudo="-ms-reveal" id="passwrod-reveal" style="display: none;"></div>
2 - enter writing password and showing "eye" icon
dom = < div pseudo="-ms-reveal" id="passwrod-reveal"></div>
3 - exit password input, click anywhere or control
div = display:none
4 - again enter password input
div = display:none

Doesn't reappear after first time use.
Note: If I completely erase the password entry and start typing again, the "eye" icon showing. This means that the icon will appear if the entry is completely blank and changes when the first character is entered. But in this case we have to delete the entry and rewrite it.

Screen Record -> 
![reveal-issue-ionic](https://user-images.githubusercontent.com/3239339/100489172-c0037300-3123-11eb-9608-69421c58aea8.gif)


html file -> 
![reveal-issue-code](https://user-images.githubusercontent.com/3239339/100489017-c2b19880-3122-11eb-88fa-5d2fbc45cdd0.jpg)


# Bug Report

**Ionic version:**
[ ] **4.x**
[x] **5.x**

**Ionic info:**
<!-- (run `ionic info` from a terminal/cmd prompt and paste output below): -->

```
Ionic:

   Ionic CLI                     : 6.12.2 (C:\Users\mhy\AppData\Roaming\npm\node_modules\@ionic\cli)
   Ionic Framework               : @ionic/angular 5.5.1
   @angular-devkit/build-angular : 0.1100.2
   @angular-devkit/schematics    : 10.0.8
   @angular/cli                  : 10.0.8
   @ionic/angular-toolkit        : 2.3.3

Capacitor:

   Capacitor CLI   : 2.4.3
   @capacitor/core : 2.4.3

Utility:

   cordova-res : 0.15.2
   native-run  : 1.2.2

System:

   NodeJS : v14.15.0 (C:\Program Files\nodejs\node.exe)
   npm    : 6.14.9
   OS     : Windows 10
```
