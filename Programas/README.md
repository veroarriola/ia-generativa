# Requerimientos

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

