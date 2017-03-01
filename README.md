nativescript-template-sumo
==========================

### Create
Create new project
```bash
tns create firstApp --template https://github.com/xmlking/nativescript-template-sumo
```

### Post Create 
move `app/webpack.common.js` into the project root.(replace)

Test your setup

`yarn run start-ios-bundle`

after **css** created, uncomment following lines in `webpack.common.js`

```js
entry['app.css'] = './app.' + platform + '.css';
{ from: './app.' + platform + '.css' },
```
