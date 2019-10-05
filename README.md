# AngularMaterialStarter

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 6.2.4.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Step-by-Step

### CLI-Commands

``` bash
ng new angular-material-starter 

cd angular-material-starter

npm install --save @angular/material @angular/cdk @angular/animations hammerjs

ng g module material --spec false
```

### Additional Edits

Add BrowserAnimationsModule to imports

<details>
    <summary>app.module.ts</summary>

``` javascript

import { BrowserModule } from '@angular/platform-browser';
import { NgModule } from '@angular/core';
import {BrowserAnimationsModule} from '@angular/platform-browser/animations';
 
import { AppComponent } from './app.component';
 
@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule,
    BrowserAnimationsModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }

```
</details>



add import statement on top of main.ts

<details>
    <summary>main.ts</summary>

```javascript
import 'hammerjs';
```
</details>


add material icons to index.html

<details>
    <summary>index.html</summary>

```javascript

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>AngMaterialOwnerAccount</title>
  <base href="/">
 
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="icon" type="image/x-icon" href="favicon.ico">
  <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
</head>
<body>
  <app-root></app-root>
</body>
</html>

```
</details>

