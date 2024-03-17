# Script ksdeps

[English version](./README.en.md)

Este es un script que tiene el propósito de generar el archivo kls-classpath a partir de un script Kotlin para kscript, usando un función no oficial del propio comando de kscript (`kscript --dependencies <script kotlin>`), el cual se propuso en esta [PR](https://github.com/kscripting/kscript/pull/420).

## Ejecución

```bash
/path/to/script/ksdeps <script kotlin>
```

## Puntos a tomar en cuenta

Este script recoge las dependencias devueltas por kscript y añade tanto el stdlib de kotlin como se ejemplifica [aquí](https://github.com/fwcd/kotlin-language-server/tree/main?tab=readme-ov-file#figuring-out-the-dependencies) y las anotaciones de metadatos para los scripts de kscript, sobre esto mas información [aquí](https://github.com/kscripting/kscript?tab=readme-ov-file#script-configuration).
