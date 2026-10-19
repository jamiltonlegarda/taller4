# Scrum y Trunk-Based Development (TBD)

Plantilla de trabajo para que el equipo acuerde cómo planifica, desarrolla e integra cambios de forma frecuente y segura.

## Principios

- Mantener una única rama principal, siempre en estado integrable.
- Integrar cambios pequeños y frecuentes para reducir conflictos y detectar problemas pronto.
- Trabajar en ramas de vida corta; evitar ramas de larga duración y lotes grandes de cambios.
- Usar Feature Toggles para integrar código incompleto sin exponer funcionalidad no habilitada.
- Automatizar las pruebas y validaciones para obtener retroalimentación rápida.
- Compartir la responsabilidad por la calidad, el producto y la estabilidad de la rama principal.

## Roles

- **Product Owner:** prioriza el Product Backlog, aclara el valor esperado y valida los criterios de aceptación.
- **Developers:** convierten las historias en incrementos terminados; diseñan, implementan, prueban y los integran a la rama principal.
- **Scrum Master:** facilita los eventos de Scrum, ayuda a eliminar impedimentos y promueve el cumplimiento de los acuerdos de trabajo.
- **Revisor o responsable de integración:** cuando el equipo lo requiera, facilita la revisión o el soporte de integración sin crear una cola prolongada de cambios.

## Reglas de Oro

- Mantener los cambios pequeños, revisables y enfocados en una historia o tarea.
- Integrar a la rama principal al menos una vez al día; no acumular trabajo en ramas de larga vida.
- Mantener la rama principal verde: si una validación falla, atenderla antes de continuar integrando cambios.
- Proteger funcionalidades incompletas o riesgosas con Feature Toggles; definir quién puede activarlos y cómo retirarlos.
- Hacer revisión colaborativa y oportuna; la revisión no debe convertirse en un bloqueo prolongado.
- Comunicar de inmediato los bloqueos, conflictos y riesgos que afecten la entrega.
- Acordar explícitamente cualquier excepción al flujo de integración y darle seguimiento hasta cerrarla.

## Definition of Done (DoD)

Una historia o cambio está terminado cuando:

- [ ] Cumple todos sus criterios de aceptación verificables.
- [ ] El código fue revisado según el acuerdo del equipo y está integrado en la rama principal.
- [ ] Las pruebas automatizadas pertinentes pasan y las nuevas pruebas necesarias están incluidas.
- [ ] El pipeline de CI pasa sin errores.
- [ ] La funcionalidad incompleta o no habilitada está protegida por el Feature Toggle definido.
- [ ] La documentación y las notas operativas se actualizaron cuando corresponde.
- [ ] No quedan defectos conocidos que impidan usar el incremento de forma segura.

## Definition of Ready (DoR)

Una historia está lista para entrar al trabajo cuando:

- [ ] Está redactada con el formato: Como [tipo de usuario], quiero [capacidad], para [beneficio].
- [ ] Sus criterios de aceptación son claros y verificables.
- [ ] Está dividida en un incremento integrable en un día o menos.
- [ ] El Feature Toggle está identificado o se indica por qué no aplica.
- [ ] No tiene dependencias bloqueantes sin resolver.
- [ ] La estrategia de pruebas automatizadas indica qué probar y dónde.
- [ ] El equipo entiende el alcance y puede estimar el trabajo.

## Acuerdos de Planificación (Taller 4)

**Pregunta de cierre:** ¿Qué cambia en nuestra próxima Planning?

**Respuesta del equipo:** El DoR estricto y el primer ítem integrable el Día 1.

### Acciones concretas

1. Aplicar el DoR estricto a cada historia antes de incorporarla al Sprint.
2. Redactar el Sprint Goal en formato TBD, indicando qué se despliega y qué queda detrás de un Feature Toggle.
3. Reservar el 30% de la capacidad del equipo para revisión de PRs y CI.
