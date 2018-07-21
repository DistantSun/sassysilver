# SassySilver

## Introduction
SassySilver is a prosilver-based style for phpBB 3.2.x seeking to combine the basic structure and layout of prosilver with the advanced possibilities SASS can offer.

In order to keep future updating as effortless as possible SassySilver makes extensive use of template inheritance and of the original prosilver stylesheets.
As far as stylesheets are concerned SassySilver's theme folder contains stylespecific stylesheets only.

###### A fee notes ...
- SassySilver is still under development. Although most of the features already implemented passed tests to insure their functionality, there still is a chance you may encouter flaws as the code gets more and more complex with each new option added during the development process.
- Some more feature may still be added to SassySilver until it reaches RC status and a few other may still change the moment they hit limits in functionality not foreseeable at the moment. Those adjustments will nevertheless focus on keeping the existing switches and usage of variables untouched as far as possible, but no garantee can be given at the current state (ALPHA or BETA releases).
- A dedicated FAQ/How-to file will be included in the near future.


## System Requirements
- based on prosilver => prosilver must be installed for this style to work!
- phpBB >= 3.2.1
- SASS Pre-Processor (see http://sass-lang.com/install for further information) supporting full SASS syntax/functionality (1)

## Install / Update
- #### Installation
    - Download the archive, unpack it locally
    - Upload the "sassysilver" folder into the "/styles/" folder of your phpBB installation
    - Actvate style via ACP
    - Re-compile stylesheets
    - Clear caches

- #### Update
    - Backup your current installation's files and folders
    - Download the archive, unpack it locally
    - Open the resulting `sassysilver` folder, go to `/theme/` and delete both `_custom_configuration.scss` and `_custom.scss` (these two files are to contain your personal/custom settings and codes you may want to keep)
    - Check your `_custom_configuration.scss` for potential changes in the naming of variables and/or for additional samples
    - Upload the remaining files and folders into the "/styles" folder on the server
    - Re-compile stylesheets
    - Clear caches


### Credits
The development of this style was inspired by the outstanding phpBB 3.0/3.1 styles by Arty (https://www.artodia.com/) introducing the potential of SASS in creating highly flexible and configurable phpBB styles.
Myself being far away from his skills SassySilver is NOT inteded to be a copy of his works but a first step to dig into the possibilities SASS may offer.

Credits go as well to all those who helped me during the development process, either by testing SassySilver or pointing me to flaws made or inconsistencies left in the code.
(Special thanks go to Talk19zehn for proof-reading the code, numerous hints to alternative approaches and sharing her knowledge.)


## Features
- #### Build in
- [x] Pre-defined colour schemes - switch between them by adjusting one setting/option only
- [x] Secondary colours will be automaticly calculated based on the choosen colour scheme
- [x] Display of mini-profile switchable left <> right
- [x] Option to split off headerbar and main menue to display it above the board wrapper
- [x] Option to split display of mini-profile and postbody and show them side by side in separate DIVs
- [x] Option to display a background image in forum body and then select between images by simply changing the image name in the corresponding cofig variable (sample images included)
- [x] Dito regarding background image in board wrapper (sample images included)
- [x] Option to switch opacity of background colour in board wrapper on or off, opacity level configurable as well (these switches will only take effect when backround images for board wrapper are turned off)

- #### Planned
- [ ] Option to set width of mini-profile to a fixed value in resolutions beyond 1280px - the corresponding width of postbody will be calculated accordingly
- [ ] Option to display and easyly change background image in headerbar
- [ ] Sidebar right, switchable to visible <> hidden


## Sidenotes
###### (1) Compatibility issues with SASS Compilers:
1. Arty's SASS Compiler Extension:<br />
This extension will fail to compile the stylesheets of this style correctly. This is not(!) due to it being badly programmed or flawed but to its original use case: providing a tool to compile his styles from within phpBB's ACP in order to avoid users having to install a dedicated piece of software for this job.<br />
There is not much I can do as far as this extension is concerned without having to re-arrange the folder/file stucture of the style in a way that will render it cluttered and, in consequence, "hard to read" and hard to manage.<br />
Therefore support for this extension will **not** be provided.

2. Koala:<br />
Koala is a different case as it will fail only in its standard configuration (as provided "out of the box"). In order to to make Koala work with this style you would have to create a dedicated configuration file and manually adapt it first<br />
Sounds like a task not really trivial? In fact it isn't ... but this is nothing uders will have to cope with:<br />
This style will be shipped with a dedicated configuration file ("koala-config.json"), located in the root of the style's folder, which should take care of this issue.<br />

3. Editor specific compiler add-ons:<br />
There are numerous add-ons for a wide range of editors providing a means to compile SASS files from within the respective editor, some of them more and others less sophisticated. Those suitable for the job of compiling this style will most likely have to be configured accordingly.<br />
Please understand that information on how to accomplish this cannot be provided.

###### (2) Third Party Packages included:

For the time being a complete set of Bourbon files will be included in the theme folder. This may change during the development process to reduce the amount of code shipped as soon as feasible.

###### (3) Additional copyrights:

Please note that SassySilver, in its current state, makes use of (external) material (e.g. sample images, Bourbon library) to which additional third party copyright/license regulations may apply.
For further information please read the corresponding license files provided with this style within their corresponding folders:
- [Bourbon](./theme/assets/bourbon/LICENSE.md/ "Bourbon MIT license") see "/SassySilver/theme/assets/bourbon/LICENSE.md""


[![Waffle.io - Columns and their card count](https://badge.waffle.io/DistantSun/sassysilver.svg?columns=all)](https://waffle.io/DistantSun/sassysilver)
