# Parte 02 - Numeracion Equipotencial y Borneras

<p align="center">
  <img src="portada-02.png" width="100%">
</p>

Como numerar correctamente un esquema electrico y como usar las borneras en CADe SIMU.

## Ver el video

Video de esta parte: [PEGA-AQUI-EL-LINK](https://youtu.be/3zHdyqJfxOc?si=6UxhK6TUAOfg9PO_)

Playlist completa del curso: https://www.youtube.com/playlist?list=PL12Fo7Tlkoigvi0rdW3g-1iNB54jVpZp-


## Que encontraras aqui

Un archivo para que practiques:

| Archivo | Para que sirve |
| --- | --- |
| `ejercicio-numeracion.cad` | Circuito de ejemplo para activar y desactivar la numeracion de cable |

## El truco de esta parte

CADe SIMU numera los cables por ti, pero viene desactivado. Se activa asi:

**Paso 1.** Menu **Archivo**

**Paso 2.** Entra a **Configuracion**

**Paso 3.** Marca donde dice **Visualizar numero de cable**

Listo. Ahora el programa te muestra el numero de cada cable sobre el esquema.

## Ejercicio

Haz lo mismo dos veces con el mismo archivo y compara.

**Primera vuelta - sin numeros**

- Abre `ejercicio-numeracion.cad` con la opcion desactivada
- Dale simular
- Sigue con el dedo por donde pasa la corriente
- Anota en un papel cuales puntos crees tu que son el mismo potencial

**Segunda vuelta - con numeros**

- Activa **Visualizar numero de cable**
- Vuelve a simular
- Ahora si ves el numero de cada cable

Ahora compara con lo que anotaste. Los puntos que tu marcaste como el mismo
potencial, quedaron con el mismo numero? Ahi es donde de verdad se entiende
la numeracion equipotencial.

No te saltes la primera vuelta. Si abres el archivo viendo los numeros de una
vez, no aprendes nada: solo estas leyendo la respuesta.

## La regla de oro

Todos los puntos unidos por cable, sin ningun elemento en medio, son el
MISMO potencial y llevan el MISMO numero.

El numero solo cambia cuando la corriente atraviesa algo: un contacto,
una bobina, un fusible, un termico.

Referencia rapida en el circuito de potencia:

| Marca | Donde va |
| --- | --- |
| L1 L2 L3 | Entrada de red |
| 1 3 5 | Bornes superiores del contactor |
| 2 4 6 | Bornes inferiores del contactor |
| U V W | Llegada al motor |

## Designacion de componentes (IEC)

| Letra | Componente |
| --- | --- |
| Q | Aparatos de maniobra de potencia (seccionador, ITM, guardamotor) |
| KM | Contactor |
| KA | Rele auxiliar |
| KT | Temporizador |
| FU | Fusible |
| FR | Rele termico |
| SB | Pulsador |
| SA | Selector |
| SQ | Final de carrera |
| B | Sensores y captadores |
| HL | Lampara de señalizacion |
| HA | Sirena, alarma sonora |
| M | Motor |
| T | Transformador |
| X | Bornes y borneras (XT) |
| W | Cables y conductores |

## Plantilla de bornera

Llena esta tabla con tu propio circuito. La bornera es lo que separa el
tablero del campo: todo lo que entra o sale del gabinete pasa por ahi.

| Borne | Viene de | Va hacia | Numero equipotencial |
| --- | --- | --- | --- |
| XT-1 | | | |
| XT-2 | | | |
| XT-3 | | | |
| XT-4 | | | |

## Material de apoyo externo

Estos documentos NO son mios y no estan alojados en este repositorio.
Son de acceso publico y aqui solo los enlazo, dando credito a sus autores.
Te sirven para comparar lo del video con normas y planos reales.

**Normalizacion y simbologia electrica** - Govern de les Illes Balears
Es el que mas se parece a lo que vimos. Trae la codificacion de conductores:
L10, L11, L12 para fases; N5, N6, N7 para neutro; PE1, PE2, PE3 para tierra.
https://sarreplec.caib.es/pluginfile.php/14797/mod_resource/content/9/IEB08/Normalizacion_simbologia_electrica.pdf

**Normas de representacion de esquemas electricos** - Tecnicsuport / Universidad de Oviedo
Basado en UNE-EN 60439-1, 60073 y 60204-1. Lo bueno es que separa lo que es
norma obligatoria de lo que es simple recomendacion de taller.
http://isa.uniovi.es/docencia/IngdeAutom/transparencias/Normas%20de%20Representacion.pdf

**Estandarizacion de esquemas** - Schneider / Telemecanique (Institut Obert de Catalunya)
Basado en la norma IEC 1082-1. Explica como se ordenan los circuitos de mando
y de señalizacion dentro del esquema.
https://ioc.xtec.cat/materials/FP/Recursos/fp_iea_m01_/web/fp_iea_m01_htmlindex/WebContent/u1/media/simbolos_electrotecnia_iec_1082-1.pdf

**Esquemas electricos ABB SACE** - catalogo tecnico de fabricante
Planos industriales reales. Fijate en los bornes marcados X1, X2, XA1, XA2:
es la misma letra X que usamos en el video, pero en un documento comercial.
https://library.e.abb.com/public/48a001fa95986ad1c1256d18005586a3/Capitulo04.pdf

**Simbologia y esquemas de motores**
https://instrumentacionycontrol.net/Descargas/IyCnet_Simbologia_y_Esquemas_Motores.pdf

> Si estas en Colombia, recuerda que la norma de obligatorio cumplimiento es
> el RETIE. Consultalo siempre en el sitio del Ministerio de Minas y Energia
> y verifica que sea la version vigente.

[<- Volver al inicio](../README.md)
