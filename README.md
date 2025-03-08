# **VIPM-Personal-Guide**

This is a work in progress guide for writing packages in VIPM, using version control in git.

The main directory looks like this:

![Directory](Images/Directory.png)

- Build folder contains this is the \*.vipb file
- Package folder contains these are the \*.vip files
- Source folder contains the source code such as \*.lvproj and folders with classes / controls / methods

# **Build**

![Build](Images/Build.png)

## Process of Building

1. Name the Build in relation to what your git repo is named, with spaces
2. File Directory to choose is the Source folder, as previously mentioned

### Build Information

![Build Information](Images/Build%20Information.png)

### Display Information

![Display Information](Images/Display%20Information.png)

### Palettes

![Palettes](Images/Palettes.png)

#### Object Drop Functions Palette

Note the same can be done for the `Controls Palette`, just replace the following `Block Diagram` with `Front Panel`.

![Object Drop Function Palette](Images/Object%20Drop%20Function%20Palette.png)

Ah, how to have an object drop on the block diagram?

This is simple by
1. creating a \*.vi
2. place the object constant on the block diagram
    <br>
    ***Side Step to updating \*.vi icon***
    1. copy image, paste into Paint program, resize from 48x48 pixels to 32x32 pixels, save as \*.png, go back to LabVIEW \*.vi, edit icon<br>
    2. `Edit >> Clear All...`
    3. `Edit >> Import Glyph from File...` and selct file
3. Back in build, place this in into the functions palette
    <br>
    *Right click empty space and select `Insert >> Control or VI...`, followed by the \*.vi you just made*
    <br>
    ![Function Place VI Contents](Images/Function%20Place%20VI%20Contents.png)
    <br>
    `Edit VI Title` to be that of the object name, such as `Class.lvclass`