# curriculum-vitae

**Código fuente de mi currículum hecho con [AwesomeCV](https://github.com/posquit0/Awesome-CV)**

## Dependencias

Para utilizar esta plantilla es necesario: 

- Un compilador de LaTeX (por ejemplo pdflatex o xelatex).
- La tipografía FontAwesome en su versión 4 (paquete para instalarla en [ArchLinux](https://aur.archlinux.org/packages/ttf-font-awesome-4/)). 

## Compilación

Compilar haciendo uso del `Makefile` (se presume una instalación completa y actualizada de LaTeX).

```sh
make
```

## Teléfono móvil

Por motivos de privacidad, mi número de teléfono aparece como `NOMOBILEPHONE`.
Para añadirlo editar el comando `\mobile{NOMOBILEPHONE}` en `src/cv.tex` o sustituir con `sed`:

```sh
mobilephone="(+34) 805551337"
sed -i 's/NOMOBILEPHONE/'"$mobilephone"'/' src/cv.tex && make; sed -i 's/'"$mobilephone"'/NOMOBILEPHONE/' src/cv.tex
```
