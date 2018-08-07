## Style History

#### 0.5.0 (w.i.p)
- New folder structure for stylesheets (hopefully for the last time ...)
- Separation of stylesheets between core stylesheets and, respectivly, custom stylesheets, relocated to their corresponding folders (see above)
- Basic implementation of revised colour scheme system: one dedicated scheme stylesheet per colour scheme; easy integration of new schemes
- Functions/mixins to automate switching between colour schemes
- Start allocation of variables to stylesheets (still w.i.p)
- Switch between scheme specific background colour, texture and style wide defined background image
- Further relocation of code to dedicated module and component stylesheets (still w.i.p)
- Dropped support for Koala since it uses an outdated and no longer supported SASS implementation (Arty's SASS Compiler Extension is still supported and will be so as long as feasible)


#### 0.4.1 (08.03.2018)
- Bug in display of PMs fixed
- Bug in display of search results fixed
- Re-coloured marker system for PMs
- Re-build headerbar to provide for responsiveness in separate view when custom logos are inserted
- Option added to switch display of site description on<>off
- Option added to switch display location of site description betwee left, center and right
- Search box layered with z-index
- Added new (default) logo
- Logo position switchable left/center/right
- Forum & topic icons: choose between different sets of icons: <br />
standard => prosilver <br />
vector1 => with kind permission and created by Mazeltof


#### 0.4.0 (08.01.2018)
- Style updated to phpBB 3.2.2
- Code of `/modules/_posts.css` adjusted to prevent postbody and postprofile of PMs from being separated
- New file `/assets/parent/_transform.scss`: providing a more transparent way to reset certain original prosilver classes/expressions for the time being.


#### 0.3.0 (19.12.2017)
- Begin overhaul of file structure: <br />
   a) **New** sub-folder within theme root `/assets`: attempt to separate "framework-like" components from the style-specific files <br />
   b) **New** sub-folder within theme root `/assets/parent`: containing the prosilver stylesheets originally imported through prosilver's `stylesheet.css`, renamed following SASS naming convention. <br />
   c) **New** sub-folder within theme root `assets/bourbon`: holding Bourbon's fileset <br />
   d) **New** sub-folder within theme root `assets/functions`: holding non-Bourbon function files<br />
   e) **New** sub-folder within theme root `assets/mixins`: holding non-Bourbon mixin files <br />
   f) New sub-folder within theme root `assets/modules`: holding holding object-based rulesets
- Reorganisation of `stylesheet.scss` and introduction of `_assets_base.scss`to reflect the above mentioned new folder structure
- Relocation of code (functions, mixins) from style-specific stylesheets to the above mentioned folders
- Code to separate postbody/postprofile and to switch positioning of postprifile left/right re-written
- Bugfixes in responsive layout of posts corrected
- Code cleaned-up and simplified


##### 0.2.2 (06.11.2017) - internal revision
- Option/Switch to display postbody and postprofile as visually separated DIVs via config SCSS file. Code completely rebuilt
- If separated postprofile will be displayed above postbody in responsive mode
- First steps to refactor the layout of mini-profile
- Stylesheets revisioned, re-arranged and simplified
- Original stylesheets to be imported via prosilver stylesheet.css included in theme folder again (after renaming in accordance with SASS naming scheme) and dropped "_import_prosilver.scss" and "_transition.scss" (now no longer needed) in order to allow compiling with less elaborate pre-processors such as Koala etc.

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
