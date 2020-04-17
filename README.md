# Base Expo React Native Typescript with Bottom Tab

This is a simple example of a React Native application generated using Expo.

What I did was to generate two separate probjects. 1 was generated with the **"Bare workflow" minimal (Typescript)** template and the other used the **"Managed workflow" tabs** template.

> ? Choose a template:
>   ----- Managed workflow -----
>   blank                 a minimal app as clean as an empty canvas
>   blank (TypeScript)    same as blank but with TypeScript configuration
>   tabs                  several example screens and tabs using react-navigation
>   ----- Bare workflow -----
>   minimal               bare and minimal, just the essentials to get you started
> ❯ minimal (TypeScript)  same as minimal but with TypeScript configuration

I then merged the tab project into the minimal project. Moving the directories:
- assets
- components
- constants
- navigation
- screens
Merged the *package.json* and simply overwrote the *App.tsx* contents with the **tabs** version.

To get everything to work nicely with Typescript, I reformated the \*.js files by creating subdirectories with the same name as the file name, copy the file into that directoy, and renaming the file to *index.ts* or *index.tsx*. For example: *./screens/HomeScreen.js* became *./screens/HomeScreen/index.tsx*

This all works, removing the file not found errors that appear in the Visual Studio Code IDE, but this is very messy. I'm going to experiment to see if there is a better way but for now this is about a clean as I can get it.
