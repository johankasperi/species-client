# Species client
Repo for the client in project 2 in INFO490 at UIUC. This project is called "Species" where you can interact with small "Species"-circuits using an iOS application. [Please click here to get more information.](https://junokas.wordpress.com/intel-galileo-board-exploration-ii-audio-interactions-with-feedback-ecologies/)

This client is an Ionic framework iOS application. This means that you must have Ionic installed on your local environment, [please read this to get started with Ionic](http://ionicframework.com/getting-started/).

## Run instructions

Change line 4 in www/js/services.js to the url of your server (if you don't want to use the provided server):
```javascript
var socket = io('http://species-kspri.rhcloud.com');
```

Change line 22 in www/index.html to the url of your server (if you don't want to use the provided server):
```html
<script src="http://species-kspri.rhcloud.com/socket.io/socket.io.js"></script>
```

Install bower modules:
```bash
bower install
```

Run in your browser:
```bash
ionic serve
```

Run on a iOS simulator:
```bash
ionic emulate ios
```

Run on your device:
First you have to run
```bash
ionic build ios
```
Then open platforms/ios/Species.xcodeproj in XCode and build the app to your device from there.

## Dependencies
Ionic framework, Bootstrap, AngularJS, Cordova. Check bower.json.

## Credits
Created by [Johan Kasperi](http://kasperi.se), [Mike Junokas](https://junokas.wordpress.com) and [Aileen Bai](http://issuu.com/aileenbai/docs/aileen_bai_portfolio_05a83c8985e264).
