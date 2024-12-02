# Taller_3_p2
##Se eencuentra el notebook con los análisis realizados para llegar al modelo que se seleccionó en pycaret-optuna-mlflow__Taller3_p2.ipynb y en el archivo MLFlow_Optuna_Taller3_p2 se encuentra el código que usa MLFLow y Optuna para usarn eEC2
Entrar a EC2, shell
Descargar el repo: git clone git@github.com:dddrra/Taller_3_p2.git
Entrar a la carpeta: cd Taller_3_p2
Crear entorno virtual: python3 -m venv taller3Venv
activar el venv: source taller3Venv/bin/activate
Instalar dependencias: pip install -r requirements.txt
Correr: python mlflow_optuna_taller3_p2.py
en EC2 Crear o editar regla de entrada en grupos de seguridad en tcp, intervalo puertos 5000
En EC2 ir a buscar la url pública, acceder, quitar la 2 de https y al final poner:5000
Para visualizar los resultados ejecutar: sudo ufw allow 5000/tcp
luego: mlflow ui --host 0.0.0.0 --port 5000

