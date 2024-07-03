# Cross-site scripting (XSS)

Cross-site scripting (XSS) es uno de los metodos mas comunes que los hackers utilizan para atacar paginas webs. Permite al usuario malicioso ejecutar codigo arbitrario JavaScript cuando otros usuarios visitan la página.

XSS es una de las vunerabilidades que más se reportan en los sitios web. 

¿Qué puede hacer un hacker explotando una vulnerabilidad XSS?

XSS ejecuta arbitrariamente codigo JavaScript, el daño que puedan hacer depende de la sensibilidad de los datos que pueda proveer dicha página.

- Se podrían difundir gusanos en las páginas como "Facebook, Twitter"
- Robo de sesión, pudiendo coger las cookies remotamente.
- Robo de identidad, Información confidencial tarjetas, numeros, etc.
- Denegación de servicio.
- Robo de datos sensibles, como contraseñas.
- Fraude financiero en bancos.

# Protección 

Para poder ser protegido por estos ataques, tendremos que tener seguros que nuestro contenido dinamico que puedas enviar datos, puedas inyectar codigo JavaScript.

Todas las páginas estan hechas con HTML, usualmente describen el tema y los ficheros, lo utilizariamos con contenido dinamico y cuando la pagina se volivera a cargar parariamos.

Con "Stored XSS attacks" hacemos que dentro del contenido dinamico podamos guardan contenido en el "backend". El atacante abusa de 
