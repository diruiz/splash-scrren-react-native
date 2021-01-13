# splash-scrren-react-native

ver para mas info:
https://github.com/bamlab/react-native-make/blob/master/docs/set-splash.md

Pasos:
0. Agregar "@bam.tech/react-native-make": "^3.0.0", a los dev dependencies

1. instalar Paquetes:
```
npm i react-native-splash-screen
npm i
```
2. importar paquete en App

```js
import SplashScreen from 'react-native-splash-screen';
```
3. agregar useEfect en App:

```js
useEffect(()=>{
    setTimeout(SplashScreen.hide, 1000);
  },[]);
```
4. Generae Splash Screen
 
 ### Generate iOS splashscreen
Abrir el archivo myProject.xcworkspace in XCode
right-click on your project folder > "New file..." > "Launch Screen" > "Save as: SplashScreen"
react-native set-splash --platform ios --path <path-to-image>
 
 ### Generate Android splashscreen
Ejecutar en la consola:
```
npx react-native set-splash --platform android --path <path-to-image> --resize <[contain]|cover|center> --background ">background-color>"
```
⚠️ The path option is mandatory.

para este ejercicio:

```
npx react-native set-splash --platform android --path ./src/assets/images/splash-screen.png --resize center --background "white"
```


