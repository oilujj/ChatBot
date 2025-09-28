# ChatBot

## 1. Instalar Python

Asegúrate de tener Python 3.12 (o superior) instalado. Puedes descargarlo desde:  
https://www.python.org/downloads/

Durante la instalación, marca la opción "Add Python to PATH".

---

## 2. Clonar o copiar el proyecto

Coloca todos los archivos del proyecto en una carpeta, por ejemplo:  
`C:\Users\TuUsuario\Desktop\ClaseAI\chatbot`

---

## 3. Crear y activar un entorno virtual

Abre PowerShell y navega a la carpeta del proyecto:
```powershell
cd C:\Users\TuUsuario\Desktop\ClaseAI\chatbot
```

Crea el entorno virtual:
```powershell
python -m venv .venv
```

Actívalo:
```powershell
.venv\Scripts\Activate
```

---

## 4. Instalar las dependencias

Con el entorno virtual activado, instala los paquetes necesarios:
```powershell
pip install -r requirements.txt
```

Esto instalará:
- `google-generativeai`
- `python-dotenv`

---

- La API Key la obtienes desde Google AI Studio.
- El modelo lo puedes listar usando la función `GeminiClient.listar_modelos(api_key)`.

---

## 5. Ejecutar el programa

Con el entorno virtual activado, ejecuta el chatbot:
```powershell
python main.py
```

---

## 6. (Opcional) Listar modelos disponibles

Para saber qué modelos puedes usar, ejecuta este fragmento en un archivo o en el intérprete interactivo:
```python
from config import settings
from llm_client import GeminiClient

GeminiClient.listar_modelos(settings.api_key)
```

---

¡Listo! Así tendrás todo instalado y funcionando como nuevo usuario. ¿Te gustaría que te ayude con algún paso específico?
