# 📚 Goodreads Top Books Filter

Este proyecto contiene un cuaderno Jupyter que realiza **scraping de listas públicas de Goodreads**, como ["Best Books Ever"](https://www.goodreads.com/list/show/1.Best_Books_Ever), para ayudarte a descubrir los libros mejor valorados según filtros personalizables.

## ✨ Funcionalidades

- Extrae datos directamente de Goodreads usando `requests` y `BeautifulSoup`.
- Permite configurar:
  - ✔️ Puntuación mínima (`MIN_RATING`)
  - ✔️ Número mínimo de valoraciones (`MIN_RATINGS_COUNT`)
  - ✔️ Tiempo de espera entre peticiones (`DELAY`)
- Muestra los libros filtrados en una tabla interactiva con `pandas`.
- Diseño pensado para ser **respetuoso con el sitio web**: incluye headers personalizados y control de la frecuencia de acceso.

## 📦 Requisitos

El cuaderno instala automáticamente las dependencias necesarias, pero puedes hacerlo manualmente con:

```bash
pip install requests beautifulsoup4 pandas
```

## 🚀 Cómo usarlo

1. Abre el cuaderno `grscraping.ipynb` en JupyterLab o Google Colab.
2. Ejecuta las celdas una por una.
3. Ajusta los parámetros al inicio del notebook:
   ```python
   URL = "https://www.goodreads.com/list/show/1.Best_Books_Ever"
   MIN_RATING = 4.3
   MIN_RATINGS_COUNT = 10000
   DELAY = 3  # en segundos
   ```
4. Visualiza los resultados en forma de tabla.

## ⚠️ Aviso legal

Este proyecto es únicamente con fines educativos. Goodreads puede tener restricciones en sus términos de uso respecto al scraping.  
**Usa este código bajo tu propia responsabilidad** y revisa las políticas del sitio antes de utilizarlo.

## 📝 Licencia

Este proyecto está licenciado bajo la [MIT License](LICENSE).

---

*Desarrollado por Fernando Pisot – Julio 2025*
