# Cómo analizar Twitter
Vamos a ver como se pueden analizar los datos de Twitter obteniendolos con dos programas: t-hoarder y twarc2

## Pedir acceso a la API de Twitter
### Acceso esencial
Lo primero de todo es solicitar acceso esencial a la API de Twitter. Esto es suficiente para poder trabajar con twarc2, aunque vamos a priorizar t-hoarder porque tiene una opción muy útil que twarc2 no tiene. Lo hacemos con el siguiente enlace:
* [Pedir acceso esencial](https://developer.twitter.com/en/portal/petition/essential/basic-info)

El proceso es muy sencillo, tenemos que decir qué uso le vamos a dar a la API y aceptar los términos y condiciones. Por último creamos una app y guardamos sus claves en un archivo de texto. Es muy importante guardar las claves porque twarc2 nos las pedirá más adelante. Si las perdemos se pueden regenerar fácilmente.

### Acceso elevado
Para poder usar t-hoarder necesitamos acceso elevado o académico. Este programa usa la API v1.1, que solo se puede acceder mediante esos dos tipos de acceso. El acceso esencial solo nos permite usar la API v2, que es con la que trabaja twarc2. Para obtener el acceso elevado o académico (mayores requisitos) usamos este enlace:

* [Pedir acceso elevado](https://developer.twitter.com/en/portal/petition/standard/basic-info)

Una vez tengamos el acceso elevado tenemos que crear una app de la API v1.1 de Twitter. En el menú de la izquierda nos vamos a "Standalone App" y creamos una. Si lo hacemos en el proyecto principal usará la API v2 y no nos servirá para t-hoarder. Por último guardamos todas las keys y tokens en un archivo de texto.

* [Información detallada sobre los tipos de acceso](https://developer.twitter.com/en/docs/twitter-api/getting-started/about-twitter-api)
### Resumen tipos de acceso
- Esencial: hasta 500.000 tweets mensuales. Tweets con antigüedad de 6 días. API v2 - twarc2

- Elevado: hasta 2 millones de tweets mensuales. Tweets con antigüedad de 6 días. Api v1.1 y API v2 - twarc2 y t-hoarder

- Académico: hasta 10 millones de tweets mensuales. Sin límite de antigüedad. Api v1.1 y API v2 - twarc2 y t-hoarder


## Obtener datos con t-hoarder
Por lo fácil que es recomiendo usar t-hoarder con esta máquina virtual linux donde viene ya instalado:
* [Tutorial para instalar máquina virtual](https://www.dropbox.com/s/j0p26bmgmct3vll/como_instalar_VM_taller_datos_twitter.pdf?dl=0)
<br />

### Configurar t-hoarder
Una vez que tengamos la máquina virtual instalada y una app que funcione con la API v1.1 podemos pasar a la configuración de t-hoarder. Para ello tenemos que enlazar el programa con la app. Vamos a "Carpeta personal de tallerdatos" -> "t-hoarder kit" -> "keys" y creamos un archivo de texto "nombre.key". En la primera línea pegamos la "public key", clicamos intro y en la segunda línea pegamos la "private key". Guardamos y cerramos.

