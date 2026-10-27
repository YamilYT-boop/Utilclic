# UtilClic

**Sitio:** https://yamilyt-boop.github.io/Utilclic/ · **Contacto:** utilclic.contacto@gmail.com

Herramientas gratis para estudiantes, en español. Todo se procesa en el navegador: los archivos nunca se suben a un servidor.

## Herramientas

| Página | Qué hace |
|---|---|
| `apa-formato.html` | Convierte un Word (.docx) a formato APA 7: portada (estudiante, profesional o institucional), márgenes, interlineado doble, niveles de título 1–5, figuras y tablas numeradas, citas en bloque, notas al pie y referencias con sangría francesa. Antes de descargar, analiza el documento y compara las citas del texto con la lista de referencias. |
| `citas-apa.html` | Generador de referencias y citas APA 7: libro, artículo, página web, capítulo, tesis, video, periódico, informe, ley o decreto, red social, software, IA (ChatGPT) y entrevista (comunicación personal). Autocompleta por DOI con Crossref. |
| `mayusculas-apa.html` | Convierte títulos a tipo oración o tipo título. |
| `lista-apa.html` | Lista de verificación APA antes de entregar. |
| `unir-pdf.html` | Une varios PDF en uno. |
| `dividir-pdf.html` | Extrae o quita páginas de un PDF. |
| `imagenes-a-pdf.html` | Convierte imágenes a PDF (Carta, A4 o tamaño de la imagen). |
| `contador-palabras.html` | Cuenta palabras, caracteres, oraciones, párrafos y páginas APA aproximadas. |

Guías: `como-citar-pagina-web-apa.html` y `portada-apa.html`.

## Cómo probarlo en tu computadora

Es un sitio estático, sin compilación. Abre `index.html` en el navegador o, mejor, levanta un servidor local en la carpeta:

```bash
python -m http.server 8000
```

y entra a <http://localhost:8000>.

## Publicarlo con GitHub Pages

1. En el repositorio: **Settings → Pages**.
2. En **Source** elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`.
3. Guarda. En uno o dos minutos el sitio queda en `https://yamilyt-boop.github.io/Utilclic/`.

## Estructura

```
index.html            Inicio
*.html                Una página por herramienta o guía
404.html              Página de error
vendor/               Librerías y fuente, servidas desde el propio sitio
```

## Librerías incluidas (`vendor/`)

- [mammoth.js](https://github.com/mwilliamson/mammoth.js): lee archivos .docx (licencia BSD-2-Clause)
- [docx](https://github.com/dolanmiu/docx): genera archivos .docx (licencia MIT)
- [pdf-lib](https://github.com/Hopding/pdf-lib): une, divide y crea PDF (licencia MIT)
- [Bricolage Grotesque](https://fonts.google.com/specimen/Bricolage+Grotesque): tipografía (licencia SIL Open Font License)

## Pendiente

- Si se activan anuncios, añadir un aviso de cookies y actualizar `privacidad.html` antes de activarlos.
