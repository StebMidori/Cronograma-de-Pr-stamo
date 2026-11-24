# Cronograma de pagos del préstamo

Calculadora web de cronograma de pagos con el **método francés** (cuota mensual fija), a partir de la **TCEA**.

## Funciones

- Monto, TCEA, plazo (1 a 360 meses) y fecha de desembolso editables; la tabla agrega o quita cuotas automáticamente.
- Cálculo de la TEM: `TEM = (1 + TCEA)^(1/12) − 1`.
- Cuotas redondeadas al céntimo; la última se ajusta para que el saldo final quede en cero.
- Nombres y DNI (opcional) del prestamista y del prestatario, con líneas de firma.
- Botón **Descargar PDF para imprimir** (hoja A4 con datos del préstamo, cronograma, totales y firmas).
- Los datos ingresados se guardan en el navegador (`localStorage`) del usuario.

> El cálculo no incluye seguros, comisiones ni ITF.

## Estructura

```
index.html   # página completa (HTML, CSS y JavaScript)
README.md
```

Librerías cargadas desde CDN (se requiere conexión a internet):
- [jsPDF 2.5.1](https://github.com/parallax/jsPDF)
- [jsPDF-AutoTable 3.8.2](https://github.com/simonbengtsson/jsPDF-AutoTable)

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo, `cronograma-prestamo`).
2. Sube `index.html` y `README.md` a la rama `main` (botón **Add file → Upload files**).
3. Ve a **Settings → Pages**.
4. En **Build and deployment**, elige **Source: Deploy from a branch**, rama `main`, carpeta `/ (root)`, y guarda.
5. En uno o dos minutos la página estará disponible en `https://<tu-usuario>.github.io/cronograma-prestamo/`.

## Uso local

Basta con abrir `index.html` en el navegador (doble clic).
