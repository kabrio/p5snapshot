Fxsnapshot
==========

Capture a set of images from your local token.

Install node:
https://nodejs.org/en/download/

Clone this repository into its own directory.

Install dependencies:
```
npm install
```

Capture *count* images:
```
node fxsnapshot.js <count>
```

Use custom URL (http://localhost:3301/ by default):
```
node fxsnapshot.js --url="file://..." <count>
```

Use custom folder to save outputs ("images" by default):
```
node fxsnapshot.js --folder 'myFolder' <count>
```

Use value from variable in file name (none by default):
```
node fxsnapshot.js --parameter variableName <count>
```

Show rendering process in browser (false by default)
```
node fxsnapshot.js --preview true <count>
```

Do not use Google SwiftShader instead of default WEBGL renderer (true by default):
```
node fxsnapshot.js --gpu false <count>
```


The script will work only if you use a canvas and call
$fx.preview(). Your token must be launched in parallel.
