# Ion Select Search
Adds input search functionality to `<ion-select>` component
This library was generated with [Angular CLI](https://github.com/angular/angular-cli) 

## Installation

Run `npm i ionic-select-search --save` to install this library. 

## Features

 1. Adds an input element in ion-select for easy searching among the list hundreds of records
 2. Just add a directive `idlDefault` to existing `<ion-select>` to enable searching

## Usage

After installing this package with `npm i ionic-select-search --save`, import the IonSelectSearchLibModule in your main module(app.module.ts) or your lazy-loaded module.
Eg: inside home.module.ts:

```
    import { IonSelectSearchLibModule } from 'ionic-select-search';
    
    @NgModule({
      ...
      imports: [
       IonSelectSearchLibModule //Import the main module
      ],
     ...
    })
    export class HomeModule { }
```

## Enable searching in `<ion-select>`

Use the directive `idlDefault` inside an `<ion-select>`

Note:`Currently interface are not supported. Work on "popover" and "action-sheet" interface is in progress. I will update the documents once done.`

Example: 
Inside your .html file
```html 
<ion-select idlDefault searchPlaceholder="Type to search" [(ngModel)]="myCategory">
    <ion-select-option value="1">Fruits</ion-select-option>
    <ion-select-option value="2">Vegies</ion-select-option>
    <ion-select-option value="3">Drinks</ion-select-option>
    <ion-select-option value="4">Cakes</ion-select-option>
    <ion-select-option value="5">Pulses</ion-select-option>
    <ion-select-option value="6">Dairy</ion-select-option>
</ion-select>
```

## Further help

For any questions, please raise an issue in the github repository https://github.com/Pankaj-Sati/IonSelectSearch.git   
