# Convencion de commits y trazabilidad

## Formato de mensajes de commit
tipo: descripcion breve (#numero-de-issue)

## Tipos utilizados
- feat: nueva funcionalidad
- fix: correccion de errores
- docs: cambios en documentacion
- audit: cambios relacionados con auditoria de configuracion
- release: cambios relacionados con una emision/release

## Ejemplos
- audit: agregar elementos de configuracion faltantes (#1)
- docs: mejorar documentacion del proyecto (#3)

## Flujo de trazabilidad
issue -> branch -> commit(s) referenciando issue -> Pull Request (Closes #issue) -> revision -> merge a main -> release

## Reglas
1. Todo cambio relevante debe partir de un issue.
2. El nombre de la rama debe reflejar el tipo de trabajo (audit/, docs/, feature/, fix/).
3. Los commits deben referenciar el numero de issue entre parentesis.
4. Los Pull Requests deben usar la plantilla y enlazar el issue con la palabra clave Closes.
