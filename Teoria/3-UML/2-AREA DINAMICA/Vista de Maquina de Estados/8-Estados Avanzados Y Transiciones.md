
## Estados avanzados y transiciones

Para modelar comportamiento más complejo que en una máquina de estado plana.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXeaRY2pasRVLP-dhMNAliJT8rmAU0JxvQL74F4uZkV9SpZefve1cPWBgRP9h8m8zRusMYtKnyg4NAL21gVqO63JbpFGXtIc2Sp6SYsUTn0EUkXzUgTHTC76Oo2BKVI8ejd19tbAjPtsBT5HAILR42q9fwAf?key=VReuh94fGGpJZLGsXsGdUQ)

### Palabras reservadas

- `entry`
- `exit`
- `do`

No se pueden usar como nombres de eventos y etc.

### Actividades `DO`

- Se ejecutan mientras el estado esté activo. Luego de las acciones de entrada.
- Asociadas a transiciones de finalización.

### Transiciones internas

- Nunca se sale del estado, se ejecutan acciones simplemente.
- En especial cuando no quieres hacer acciones de entrada o salida.

### Acciones `entry` & `exit`

- Útiles para entrada (configuración inicial) o salida (limpieza final).
- Sí o sí se ejecutan, no pueden tener argumentos o condiciones de guarda.
- Sin embargo, el efecto de entrada del nivel superior de una máquina de estados de una clase puede tener parámetros, para los argumentos que recibe la máquina cuando se crea el objeto.

### Diferencia entre transición interna y auto-transición

- **Auto-transición**: Un evento dispara la transición, se abandona el estado, se ejecuta una acción (si la hay), y se vuelve a entrar en el mismo estado. Como la transición sale y entra en el estado, una auto-transición ejecuta la acción de salida, después ejecuta la acción de la auto-transición y, por último, ejecuta la acción de entrada del estado.
- **Transición interna**: Queda esperando a que algo ocurra, es una transición interna cuando no se ejecutan acciones de `ENTRY` ni `EXIT`.

### Evento diferido = Deferred Event

- Escuchando eventos y aplicándolos, ante un cambio de estado se van desapilando.


![](https://lh7-us.googleusercontent.com/docsz/AD_4nXfHsYHsFy0P4ClhKimRC7QgAKfORyxvy4w_IfRujI2bpwLsg_Crw96zEpV4WvLgspPkOo2yOsCMpr5G7v0yAd_EsxN4LTfm8Ax3NXU94j2pVKo8KxfiBFcP9zKHvm_m4FJvEdNnQs5C7xcGfp6lST9fjAk?key=VReuh94fGGpJZLGsXsGdUQ)

## Estados compuestos (subestados)

Estados que a su vez poseen varios estados. **Una transición de un estado a un subestado rompe el encapsulamiento.** Pueden ser:


**Estados no ortogonales**: Un objeto puede tener un estado a la vez. Son los que más vemos. No puede haber dos estados concurrentes.

- ![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdDLKEcAONC97pKn5UFtCkgyzOOwua-r02rUgmBNtEJ77IVvTAr3CVtCIAMvoby2E8Stn3ULBRpfT0ndzhuFB-OFOIFw_l9dnkZjdbTSXz42TgFGY54lSkXub9eyKfGpJbOB8pisbdjgw4GdUamRZmonJkI?key=VReuh94fGGpJZLGsXsGdUQ)

**Estados ortogonales**: Múltiples estados simultáneos, estos tienen más sentido cuando modelamos un sistema completo.

- ![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcuUE4OEH02sv3AQ4Ns8_ZHkZuugdaA7gEbr91t3Ewbijv8xYZNcb9x6xqiI2ka3_25jDiF0FaTi0qyqBnOSHprU_mCj0fVigfJgA3Tqz7cwwhfrnCLScMTRBts2TPv_S4M3Snj9dYr1UHlbyhQS32BthIs?key=VReuh94fGGpJZLGsXsGdUQ)


