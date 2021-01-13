# splash-scrren-react-native

Pasos:
1. instalar Paquete:
```
npm i react-native-splash-screen
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


