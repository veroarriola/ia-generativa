# Requerimientos

## Paquetes básicos

En Ubuntu instalar:
```
sudo apt install python3-venv
sudo apt install python3-pip
```

A partir de Ubuntu 24.04 es necesario crear un ambiente virtual para instalar paquetes de python con ```pip```.

```
python3 -m venv ~/pyvenv/
```

Una vez creado, instalar desde el ambiente virtual:
```
source ~/pyvenv/bin/activate
pip install jupyter
```

Ejecutar ```jupyter``` desde el ambiente virtual:
```
source ~/pyvenv/bin/activate
jupyter notebook
``` 
Se puede agregar ```jupyter lab``` con:
```
pip install jupyterlab
```

## Uso de GPUS NVidia

Instalar controladores de NVidia.  La versión depende de la tarjeta gráfica, un ejemplo es:

```
sudo apt install nvidia-utils-550
sudo apt install nvidia-driver-550
```
Reiniciar la computadora.

Si la instalación fue exitosa, al inciar de nuevo será posible detectar la targeta al ejecutar:
```
nvidia-smi
```

Instalar pytorch.  En general seguir las indicaciones en [START LOCALLY](https://pytorch.org/get-started/locally/).  Para versión 12.1 de CUDA, desde jupyter:
```
!pip install torch torchvision torchaudio
```