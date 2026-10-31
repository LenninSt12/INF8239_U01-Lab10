# Evidencia de Ejecución de la Aplicación Streamlit (LAB 10)

Para capturar la evidencia visual del despliegue local de la interfaz interactiva de los modelos generativos, se ejecutó el siguiente comando en la terminal dentro del directorio raíz del proyecto:

```powershell
uv run streamlit run app/streamlit_app.py
```

## Verificación del Servicio
- **URL Local:** `http://localhost:8501`
- **Componentes cargados:** Decodificador latente (`models/decoder.keras`) para la generación y reconstrucción de prendas en tiempo real sobre el conjunto Fashion-MNIST.
- **Exportación de dependencias para nube:**
  ```powershell
  uv export --format requirements.txt --extra cpu --output-file requirements-cloud.txt
  ```

Esta ejecución garantiza que la interfaz opera correctamente sobre el entorno aislado sin conflictos con dependencias externas.