## Informe de configuración de VPS para desarrollo de algoritmos de IA

- **Objetivo:**

Configurar la VPS y probar algoritmos de IA


- **Actualización del sistema:**

 ```bash
 sudo apt update
 sudo apt upgrade -y
 ```

- **Instalación de herramientas esenciales:**

 ```bash
 sudo apt install git python3 python3-pip python3-venv
 ```


 2. **Estructura de carpetas:**

- **Carpetas raiz:**

 ```bash
 mkdir ia_models
 ```

- **Carpetas por proyecto:** Dentro de la carpeta raíz, subir las carpetas de los algoritmos


3. **Creación de entornos virtuales:**

- Navegue hasta el algoritmo y cree el entorno virtual

```bash
cd ia_models/<model_name>
python3 -m venv env 
```

- **Dentro del agoritmo, cuando se vaya a ejecutar hay que activar el entorno virtual usando:**
     
```bash
source env/bin/activate
```

- **Instalación de dependencias:**

- Instale las bibliotecas necesarias para cada proyecto dentro del entorno virtual:
       

```bash
pip install -r requirements.txt
```
     
- Si no tiene un archivo `requirements.txt`, puede instalarlo manualmente:

```bash
pip install tensorflow
pip install numpy
# ...
```

- **Dentro del directorio del algoritmo, para desactivar el entorno virtual use:**
     
```bash
deactivate
```


## Diagrama de estructura de carpetas (por algoritmos)

```
ia_models/
├── Arima
│	├── <carpeta proyectos>
│	│	├── config.json
│	│	└── interest.json
│	├── config.json
│	├── iamodels.py
│	├── main.py
│	└── requirements.txt
│
├── Chat Bot
│	├── <carpeta proyectos>
│	│	├── config.json
│	│	└── interest.json
│	├── config.json
│	├── iamodels.py
│	├── main.py
│	└── requirements.txt
│
├── Feelings Analysis
│	├── <carpeta proyectos>
│	│	├── config.json
│	│	└── interest.json
│	├── config.json
│	├── iamodels.py
│	├── main.py
│	└── requirements.txt
│
├── Grammatical Tools
│	├── <carpeta proyectos>
│	│	├── config.json
│	│	└── file.txt
│	├── config.json
│	├── iamodels.py
│	├── main.py
│	└── requirements.txt
│
├── IA Image
│	├── <carpeta proyectos>
│	│	└── config.json
│	├── config.json
│	├── iamodels.py
│	├── main.py
│	├── train.py
│	└── requirements.txt
│
├── Lineal Regresion
│	├── <carpeta proyectos>
│	│	├── config.json
│	│	└── interest.json
│	├── config.json
│	├── iamodels.py
│	├── main.py
│	└── requirements.txt
│
├── Logistic Regresion
│	├── <carpeta proyectos>
│	│	├── config.json
│	│	└── interest.json
│	├── config.json
│	├── iamodels.py
│	├── main.py
│	├── train.py
│	└── requirements.txt
│
├── Mental Maps
│	├── <carpeta proyectos>
│	│	├── config.json
│	│	└── interest.json
│	├── config.json
│	├── iamodels.py
│	├── main.py
│	└── requirements.txt
│
├── Natural Language Predictor (NLP)
│	├── <carpeta proyectos>
│	│	├── config.json
│	│	└── interest.json
│	├── config.json
│	├── iamodels.py
│	├── main.py
│	└── requirements.txt
│
├── Neural Networks
│	├── Neural networks (Binary Classification)
│	│	├── <carpeta proyectos>
│	│	│	├── config.json
│	│	│	└── interest.json
│	│	├── config.json
│	│	├── iamodels.py
│	│	├── main.py
│	│	├── train.py
│	│	└── requirements.txt
│	│
│	└── Neural networks (Binary Classification)
│		├── <carpeta proyectos>
│		│	├── config.json
│		│	└── interest.json
│		├── config.json
│		├── iamodels.py
│		├── main.py
│		├── train.py
│		└── requirements.txt
│	
├── Random Forest
│	├── <carpeta proyectos>
│	│	├── config.json
│	│	└── interest.json
│	├── config.json
│	├── iamodels.py
│	├── main.py
│	├── train.py
│	└── requirements.txt
│
├── Random Forest Recommendation
│	├── <carpeta proyectos>
│	│	├── config.json
│	│	└── interest.json
│	├── config.json
│	├── iamodels.py
│	├── main.py
│	├── train.py
│	└── requirements.txt
│
├── Recomendacion v2
│	├── <carpeta proyectos>
│	│	├── config.json
│	│	└── interest.json
│	├── config.json
│	├── iamodels.py
│	├── main.py
│	└── requirements.txt
│
├── Short Text
│	├── <carpeta proyectos>
│	│	├── config.json
│	│	└── interest.json
│	├── config.json
│	├── iamodels.py
│	├── main.py
│	└── requirements.txt
│
├── Text To Speeck
│	├── <carpeta proyectos>
│	│	├── config.json
│	│	└── interest.json
│	├── config.json
│	├── iamodels.py
│	├── main.py
│	└── requirements.txt
└──────
```
