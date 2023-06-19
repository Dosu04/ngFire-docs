# ngFire-docs
Tutorial/Docs for AngularFire Project 2023 by ME (Emmanuel Oladosu)

#Getting Started/Setup

## Navigation
### [Setup Development Environment](#1)
If you haven't installed the following:
- __VS Code__ (or any good code editor)
- __Node__
- __Angular CLI__

### [Setup Project](#2)

### [Deploy Project](#3)

&nbsp;

&nbsp;

&nbsp;

## Content
# 1
### Development Environment 
- [Download & Install VS Code](https://code.visualstudio.com/download)
- Install VS Code Extensions
  - Prettier
  - Angular Language Service
  - Angular Snippets
  - Auto rename tag
  - Auto close tag
  - CSS Peak
  - HTML CSS Support
  - Bracket pair colorizer 2
  - HTML to CSS autocompletion
  - Visual Studio Intellicode
  - VS Code Icons
- [Download Node](https://nodejs.org/pt-br/download)
- Install Angular CLI `npm i -g @angular/cli@latest`

# 2
### Project Setup
-  `ng new app-name`
-  `cd app-name`
-  `ng add @angular/material` **(optional)**
-  Add `"postinstall": "ngcc"` to your package.json file under scripts **(optional)**
-  `npm install -g firebase-tools`
-  `firebase login`
-  Navigate to [Firebase Console](https://console.firebase.com), create a new project and app
-  `ng add @angular/fire` 

# 3
### Deploy Project
`ng deploy`
