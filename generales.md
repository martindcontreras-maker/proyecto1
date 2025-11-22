## Recomendaciones generales

1. Considerar el uso de BEM:

En lugar de:

```
.administrativo
.textadministrativo
.adm1
.adm2
.imgadministrativo
```

Puede ser:

```
.administrativo (bloque)
.administrativo__texto (elemento)
.administrativo__parrafo--variante-1 (elemento + modificador)
.administrativo__parrafo--variante-2 (elemento + modificador)
.administrativo__imagen
```

2. Pensar los nombres de clases en terminos de abstracciones de diseño en vez de contenido, para que sean más reutilizables.

Por ejemplo, en lugar de:

```
.sonidista
.sonidistatitulo
.registrosporndeparticipe
.sonidistatitulo
.bloques
.sonidistaregistros
```

Puede ser

```
.experiencia (aplicable a cualquier tipo de experiencia personal o profesional)
.experiencia__titulo
.experiencia__seccion (aplicable a cualquier seccion dentro de una experiencia)
.experiencia__titulo
.galeria  (aplicable a cualquier galeria, dentro o fuera de experiencia)
.galeria__imagen
```

De esa manera podes agregar o sacar secciones de experiencia sin tener que definir nuevas clases en tu CSS, además te asegura consistencia entre secciones que son similares entre sí.