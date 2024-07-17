# jellyfin-theme-css
> [!IMPORTANT]
> JellySkin requires Chrome (105 and above), Edge (105 and above), Safari (15.4 and above), Firefox (121 and above), Opera (91 and above) and any other Browser supporting Baseline 23 css features to work properly


# ℹ️ Usage
- To use the JellySkin theme copy the line below into "Dashboard -> General -> Custom CSS" and click save, it will apply immediately server-wide to all users on top of any theme they may be using. To remove the theme, clear the "Custom CSS" field and then click save. <b>NOTE: Theme may not work when using Nginx Reverse Proxy. Scroll down below to learn how to fix this.

This is my custom CSS for Jellyfin.

1. Copy "mytheme" folder into the jellyfin themes directory (Jellyfin/Server/jellyfin-web/themes/)

2. GO to Dashbosrd -> General -> Custom CSS code, and put this line: @import 'https://github.com/abhishekdeyroy/jellyfin-theme-css/blob/main/theme.css';

3.Importan (cus this is a work in proggress)
Select Dark theme of Jellyfin (This custom css work with it).
Set 100% zoom on browser.
Uncheck Backdrops images to all user (User -> Display).






  ```css
  @import 'https://github.com/abhishekdeyroy/jellyfin-theme-css/blob/main/theme.css';
  ```

  - ### Custom

      If you need to add your own gradient use:

      ```css
      :root {
        --accent1-light: YOUR ACCENT COLOR 1(LIGHTER SHADE);
        --accent1-dark: YOUR ACCENT COLOR 1(DARKER SHADE);
        --accent1-light-opacity1: YOUR ACCENT COLOR 1(WITH OPACITY 0.4);
        --accent2-light: YOUR ACCENT COLOR 2(LIGHTER SHADE);
        --accent2-dark: YOUR ACCENT COLOR 2(DARKER SHADE);
      }
      ```
      
# 💻 Screenshots

- ### Login Page
    ![Login_Page](https://github.com/prayag17/JellySkin/assets/55829513/9ca0d0c2-9ada-4e41-93b9-e4281be20d1d)
  
- ### Home Screen
    ![Home page](https://github.com/prayag17/JellySkin/assets/55829513/075d844b-ca43-4f61-b54a-cb75110e77ed)

- ### Library
    ![Library](https://github.com/prayag17/JellySkin/assets/55829513/c3ef8e48-df17-44f0-9708-e10dfa448237)
  
- ### Title Screen
    ![Title page](https://github.com/prayag17/JellySkin/assets/55829513/270bb0bb-a755-449d-a57d-9da4e31d6082)

- ### Episodes List
    ![Episodes](https://github.com/prayag17/JellySkin/assets/55829513/eaded068-5930-47fd-b5d0-03cf89e1da44)

# ❓ Common Problem Fixes
  If you don't do this the theme will simply not load (reverts back to default theme) and the browser console will spit out an error. Even if you paste in all the CSS, the font will still not load since it is loaded from a disallowed external source.
