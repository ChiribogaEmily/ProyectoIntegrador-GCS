# Checklist de auditoria de configuracion

Este documento define los controles minimos que debe cumplir cada cambio antes de integrarse a la rama main.

## Antes de abrir un Pull Request
- [ ] El commit referencia el numero de issue correspondiente
- [ ] La rama sigue la convencion de nombres (audit/, docs/, feature/, fix/, integridad/, release/)
- [ ] No se incluyen archivos de configuracion con datos sensibles (contrasenas, tokens, claves)
- [ ] Se uso .env.example en lugar de archivos .env reales

## Antes de hacer merge
- [ ] El Pull Request usa la plantilla definida (.github/PULL_REQUEST_TEMPLATE.md)
- [ ] El PR incluye la palabra clave Closes seguida del numero de issue
- [ ] Se revisaron los archivos modificados (pestana Files changed)
- [ ] No hay archivos sueltos ni cambios fuera del alcance del issue
- [ ] El estado del PR es aprobado antes de mergear

## Despues del merge
- [ ] El issue relacionado se cerro automaticamente
- [ ] La rama de trabajo se elimino
- [ ] main quedo actualizado y estable

## Antes de un release
- [ ] Todos los issues planificados para la version estan cerrados
- [ ] main esta actualizado y sin cambios pendientes
- [ ] Se genero el tag de version correspondiente
- [ ] Las release notes documentan los cambios incluidos
