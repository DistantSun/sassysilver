## Style History

##### 0.3.0 (02.09.2017)
- Option/Switch to display postbody and postprofile as visually separated DIVs via config SCSS file
- If separated postprofile will be displayed above postbody in responsive mode
- First steps to refactor the layout of mini-profile
- CSS revisioned, re-arranged and simplified

##### 0.2.1.1 (02.08.17) - Service Release:
- Order of @import rules in stylesheet.scss adjusted to better include original prosilver stylesheets in the copiling process
- Bugfixes
- Code clean-up

##### 0.2.1 (29.07.17):
- Style updated to phpBB 3.2.1
- Added option/configuration switch to turn opacity of wrap's background colour on/off (deactivated when display of a background image in wrap is activated)
- Bugfixes
- Code clean-up

##### 0.2.0 (23.07.17):
- First ALPHA release !
- Complete overhaul of existing stylesheet scheme: only style specific stylesheets remaining in theme folder (all original stylesheets of prosilver will now be imported)

##### 0.1.4.1 (25.06.17) - Service Release:
- Modifications to general layout
- Include variables and code to provide the option to assign background images to body and wrapper via cofiguration switches
- Bugfixes
- Code clean-up

##### 0.1.3 (25.06.17):
- Option to limit displayed width of mini-profile under resolutions beyond 1100px (width of postbody will be calculated accordingly)
- Option to switch mini-profile in posts left <> right re-coded to reflect changes made nescessary due to option mentioned before
- Bugfixes, Code clean-up

##### 0.1.2 (18.06.17):
- Added option/configuration switch to switch mini-profile in posts left <> right
- Added option/configuration switch to display headerbar and nav-main either "prosilver standard" or separated from board wrapper

##### 0.1.1 (07.06.17):
- Colour mapping extended to navbar and headerbar
- Re-coding the mechanism to derive and assign secondary colours from the corresponding base value

##### 0.1.0 (05.06.17) - Inital DEV Release of SassySilver
- Renamed original prosilver stylesheets following SASS naming convetions
- Added Bourbon library
- Added option/configuration switch to change board width in configuration file
- First attempt to provide a pre-defined set of 4 colour schemes to choose from via switch in configuration file
