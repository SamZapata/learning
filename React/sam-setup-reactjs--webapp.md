# Aplicación Web con ReactJS
*by jsamzapata*

## Content...
### Estructura
- JS Code
> Index -> App -> Components { Main } => { Styles[ header.css, footer.css, ... ], Header, Footer }
- Components
> Styles: { Header, Footer } </br>
> Base: { Header, Footer, } </br>
> BusinessComponents: { ... }

### Primeros Componentes (Header - Footer)

Configuración del Header y el Footer

### Gestor de Rutas

1 - Importaciones necesarias

```
 import { Switch, Route, Redirect, withRouter } from 'react-router-dom';
``` 

2 - Configurar switch
- En *MainComponent* se estructura la respuesta de los componentes conforme a las rutas. </br>
Return del Componente *Main*
```
                 <Switch>
                    <Route path="/pathComponentA" component={ComponentA}/>
                    <Route path='/pathComponentX' component={ComponentX} />
                    <Redirect to="/" />
                </Switch>
```