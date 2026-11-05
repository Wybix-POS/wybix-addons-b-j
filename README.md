# Wybix para B&J Super

Versiones de **Wybix POS** con la marca de **B&J Super** (abarrotes, León, Gto.).

Este repositorio solo guarda los **instaladores** (GitHub Releases). El código vive en el repositorio de Wybix, en `custom-addons/wybix_bjsuper/`.

## Qué trae

- **Carri**, la mascota de B&J Super, en lugar de la mascota de Wybix: inicio, dock, guía y cobro en la caja táctil.
- El **logo** de B&J Super detrás del catálogo de la caja táctil, en el menú en línea y en la tarjeta del Club (Apple Wallet y Google Wallet).
- Colores de marca: azul `#1B2D7A` y amarillo `#FFD21F`.
- **Venta suelta** encendida desde el primer arranque: vende por pieza lo que se compra en paquete (el cigarro de la cajetilla). Se puede apagar en **Aplicaciones**.

## Instalar

1. Descarga `Wybix-Setup-bjsuper.exe` del último release.
2. Ejecútalo como administrador. Instala SQL Server Express si la computadora no lo tiene.
3. Activa la licencia del negocio. La licencia queda ligada a esa computadora.

Si la computadora ya tiene Wybix, este instalador se pone encima y conserva la base, la licencia y la configuración.

## Actualizaciones

La app de B&J busca sus actualizaciones **solo aquí**, en el canal `bjsuper` (`bjsuper.yml`). Nunca recibe el Wybix general encima.

## Publicar una versión (equipo de Wybix)

Desde el repositorio de Wybix:

```bash
npm run publish -- --addon wybix_bjsuper
```

Compila con el addon, sube el instalador y deja el release como **borrador**. Se revisa y se publica desde la página de Releases. Las notas salen de `custom-addons/wybix_bjsuper/notas/<versión>.md`.

## No subir aquí

Archivos originales de diseño (PDF, editables, fuentes) ni datos del negocio. Solo instaladores.
