# Ong Client

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app), using the [Redux](https://redux.js.org/) and [Redux Toolkit](https://redux-toolkit.js.org/) template.


### Uso de SweetAlert2

Las Alertas se encuentran Services/alerts/Alerts.js

### Modo de implementación


Importar la alerta que necesitamos entre llaves:

```
import { alertError } from '../../Services/alerts/Alerts'

```

Posee parámetros por lo que podemos manejar el error e introducirle mas información o dejarlo vacío:

```
const alertError = (textError = '') => { Swal.fire({ type: 'error', title: 'Oops...', text: textError, })}
```

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.


### 'Progress.js' 

A simple react progress bar loader component already customized, you can default import and run with the implementation of hooks.
Si se utilizan dentro de un botón tiene que ser una arrow function:


```
<button onClick={()=>alertError('ha ocurrido un error')} </button>
```




Ejemplo de uso en un catch:

```
catch (error) { alertError(error) }

```
