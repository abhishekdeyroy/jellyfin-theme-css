# jellyfin-theme-css
> [!IMPORTANT]
> JellySkin requires Chrome (105 and above), Edge (105 and above), Safari (15.4 and above), Firefox (121 and above), Opera (91 and above) and any other Browser supporting Baseline 23 css features to work properly


# ℹ️ Usage
- To use the JellySkin theme copy the line below into "Dashboard -> General -> Custom CSS" and click save, it will apply immediately server-wide to all users on top of any theme they may be using. To remove the theme, clear the "Custom CSS" field and then click save. <b>NOTE: Theme may not work when using Nginx Reverse Proxy. Scroll down below to learn how to fix this.

This is my custom CSS for Jellyfin.

> [!IMPORTANT]
> JellySkin requires Chrome (105 and above), Edge (105 and above), Safari (15.4 and above), Firefox (121 and above), Opera (91 and above) and any other Browser supporting Baseline 23 css features to work properly

- To use the JellySkin theme copy the line below into "Dashboard -> General -> Custom CSS" and click save, it will apply immediately server-wide to all users on top of any theme they may be using. To remove the theme, clear the "Custom CSS" field and then click save. <b>NOTE: Theme may not work when using Nginx Reverse Proxy. Scroll down below to learn how to fix this.

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

  
- ### Home Screen
    ![Home page](https://github.com/abhishekdeyroy/jellyfin-theme-css/blob/main/img/Home%20Screen.png)

- ### Library
    ![Library](https://github.com/abhishekdeyroy/jellyfin-theme-css/blob/main/img/Library.png)
  
- ### Title Screen
    ![Title page](https://github.com/abhishekdeyroy/jellyfin-theme-css/blob/main/img/Title%20Screen.png)

- ### Episodes List
    ![Episodes](https://github.com/abhishekdeyroy/jellyfin-theme-css/blob/main/img/Episodes%20List.png)

- ### Setting Menu
    ![Episodes](https://github.com/abhishekdeyroy/jellyfin-theme-css/blob/main/img/setting.png)

# ❓ Common Problem Fixes
  If you don't do this the theme will simply not load (reverts back to default theme) and the browser console will spit out an error. Even if you paste in all the CSS, the font will still not load since it is loaded from a disallowed external source.
