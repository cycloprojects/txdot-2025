# Street Smart Widget for Experience Builder

A simple Cyclorama Widget based on our Street Smart API.
See https://www.cyclomedia.com/ for more information on Street Smart

### Getting Started

## Developing

Run `npm start` on your server command terminal to turn on the local host server where you will be editing your Experience Builder applications.

Run `npm start` on your client command terminal which automatically transpiles your widget extensions and copies everything to `dist` of your client widget directory.

## Instructions for getting the compiled code to work in Experience Builder Developer Edition:

-Download the zip file
-Unzip the folder 'StreetSmart-ExB' to the '../client/dist/widgets' folder of your ExB files
-Open the 'widgets-info-existed.json' file of the '../client/dist/widgets' folder with a text editor
-Add this code below right before the "arcgis-map" bracket on line 2:

{
    "name": "StreetSmart-ExB",
    "manifest": {
      "name": "StreetSmart-ExB",
      "label": "StreetSmart-ExB",
      "type": "widget",
      "version": "1.12.0",
      "exbVersion": "1.12.0",
      "author": "Cyclomedia",
      "description": "A Street Smart Viewer widget for the Experience Builder.",
      "copyright": "",
      "license": "http://www.apache.org/licenses/LICENSE-2.0",
      "defaultSize": {
        "width": 320,
        "height": 400
      },
      "properties": {
        "coverLayoutBackground": true
      },
      "dependency": "jimu-arcgis",
      "translatedLocales": [
        "en",
        "ar",
        "bg",
        "bs",
        "ca",
        "cs",
        "da",
        "de",
        "el",
        "es",
        "et",
        "fi",
        "fr",
        "he",
        "hr",
        "hu",
        "id",
        "it",
        "ja",
        "ko",
        "lt",
        "lv",
        "nb",
        "nl",
        "pl",
        "pt-br",
        "pt-pt",
        "ro",
        "ru",
        "sk",
        "sl",
        "sr",
        "sv",
        "th",
        "tr",
        "zh-cn",
        "uk",
        "vi",
        "zh-hk",
        "zh-tw"
      ]
    },
    "i18nLabel": {
      "en": "StreetSmart-ExB-Widget",
      "ar": "StreetSmart-ExB-القطعة",
      "bg": "StreetSmart-ExB-Widget",
      "bs": "StreetSmart-ExB-Widget",
      "ca": "StreetSmart-ExB-Widget",
      "cs": "StreetSmart-ExB-Widget",
      "da": "StreetSmart-ExB-Widget",
      "de": "StreetSmart-ExB-Widget",
      "el": "StreetSmart-ExB-Widget",
      "es": "Widget StreetSmart-ExB",
      "et": "StreetSmart-ExB-vidin",
      "fi": "StreetSmart-ExB-Widget",
      "fr": "StreetSmart-ExB-Widget",
      "he": "StreetSmart-ExB-Widget",
      "hr": "StreetSmart-ExB-Widget",
      "hu": "StreetSmart-ExB-Widget",
      "id": "StreetSmart-ExB-Widget",
      "it": "StreetSmart-ExB-Widget",
      "ja": "StreetSmart-ExB-ウィジェット",
      "ko": "StreetSmart-ExB-위젯",
      "lt": "StreetSmart-ExB-Widget",
      "lv": "StreetSmart-ExB-logrīks",
      "nb": "StreetSmart-ExB-Widget",
      "nl": "StreetSmart-ExB-Widget",
      "pl": "Widżet StreetSmart-ExB",
      "pt-br": "Widget StreetSmart-ExB",
      "pt-pt": "Widget StreetSmart-ExB",
      "ro": "StreetSmart-ExB-Widget",
      "ru": "StreetSmart-ExB-Widget",
      "sk": "StreetSmart-ExB-Widget",
      "sl": "StreetSmart-ExB-Widget",
      "sr": "StreetSmart-ExB-Widget",
      "sv": "StreetSmart-ExB-Widget",
      "th": "StreetSmart-ExB-วิดเจ็ต",
      "tr": "StreetSmart-ExB-Widget'ı",
      "zh-cn": "StreetSmart-ExB-Widget",
      "uk": "Віджет StreetSmart-ExB",
      "vi": "StreetSmart-ExB-Widget",
      "zh-hk": "StreetSmart-ExB-Widget",
      "zh-tw": "StreetSmart-ExB-Widget"
    },
    "i18nDescription": {
      "en": null,
      "ar": null,
      "bg": null,
      "bs": null,
      "ca": null,
      "cs": null,
      "da": null,
      "de": null,
      "el": null,
      "es": null,
      "et": null,
      "fi": null,
      "fr": null,
      "he": null,
      "hr": null,
      "hu": null,
      "id": null,
      "it": null,
      "ja": null,
      "ko": null,
      "lt": null,
      "lv": null,
      "nb": null,
      "nl": null,
      "pl": null,
      "pt-br": null,
      "pt-pt": null,
      "ro": null,
      "ru": null,
      "sk": null,
      "sl": null,
      "sr": null,
      "sv": null,
      "th": null,
      "tr": null,
      "zh-cn": null,
      "uk": null,
      "vi": null,
      "zh-hk": null,
      "zh-tw": null
    },
    "uri": "widgets/StreetSmart-ExB/",
    "icon": "widgets/StreetSmart-ExB/icon.svg",
    "order": 1,
    "group": 7
  },

-Restart the client command terminal (npm start)
-Make sure the widget is showing up in the list of widgets in the custom widget section
-Add the widget to your application.

## Adding it to your Enterprise 11+:

-Once the widget is added to your application, publish the application on the top right
-Download the application using the three dots on the top right of the ExB builder
-Once the application finishes downloading, go to the '../client/dist-prod/widgets' folder of your ExB files
-There you should see a copy of the 'StreetSmart-ExB' folder that was added to your application
-Copy the widget inside of the 'dist-prod' folder and transfer it over to your Enterprise server
*Note: if you don't see the widget folder inside of 'dist-prod' then check inside of the application just downloaded for the Street Smart widget inside of there
-From there you can follow the Esri instructions to get your widget registered on your Enterprise if it is version 11+
-https://doc.arcgis.com/en/experience-builder/11.0/configure-widgets/add-custom-widgets.htm


## Versioning Format

Current version: **24.1.1**

We use YEAR.MAJOR.PATCH versioning.
i.e.: 16.1.0 = year 2016, major version 1, patch 0.

We also make use of:

Street Smart API:

*	api.version: 24.1.3
*	api.location: [Street Smart API](https://streetsmart.cyclomedia.com/api/v24.1/StreetSmartAPI.js)
* NPM Package (https://www.npmjs.com/package/@cyclomedia/streetsmart-api)


## Authors

* **Jasper Roosenmaallen** - [Jasper Roosenmaallen](mailto:jroosenmaallen@cyclomedia.com).
* **Harm Bruinsma** - [Harm Bruinsma](mailto:hbruinsmaboekema@cyclomedia.com).
* **Gijs Boekema** - [Gijs Boekema](mailto:gboekema@cyclomedia.com).
* **Sarath Chandra Kalluri** - *Initial work* - [Sarath Chandra Kalluri](mailto:skalluri@cyclomedia.com).
* **Jasper Stam** - https://github.com/stam
* **Chris Taylor** - [Chris Taylor](mailto:ctaylor@cyclomedia.com).
* **Giorgy Castaneda** - *Experience Builder Widget Developer* - [Giorgy Castaneda](mailto:gcastaneda@cyclomedia.com).

## License

This project is licensed under Commercial License.
Street Smart Widget for ArcGIS Online is a product of CycloMedia Technology B.V. This product is protected by copyright (c) 2016.
