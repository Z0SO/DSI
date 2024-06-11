
```markdown
Hola necesito que te dediques a hacer apuntes para estudiar sobre la materia DISEÑO DE SISTEMAS que sean hermosisimos en markdown para obsidian, te voy a pasar los textos de mis apuntes en docs y tu procesaras todo como te dije. vas a hacer siempre eso a menos que te indique lo contrario
```


```js
// Configuración del calendario
const calendarData = { 
    year: 2022, // Año del calendario (opcional, por defecto es el año actual)
    colors: { // Colores para las diferentes intensidades (opcional)
        blue: ["#8cb9ff", "#69a3ff", "#428bff", "#1872ff", "#0058e2"],
        green: ["#c6e48b", "#7bc96f", "#49af5d", "#2e8840", "#196127"],
        red: ["#ff9e82", "#ff7b55", "#ff4d1a", "#e73400", "#bd2a00"],
        orange: ["#ffa244", "#fd7f00", "#dd6f00", "#bf6000", "#9b4e00"],
        pink: ["#ff96cb", "#ff70b8", "#ff3a9d", "#ee0077", "#c30062"],
        orangeToRed: ["#ffdf04", "#ffbe04", "#ff9a03", "#ff6d02", "#ff2c01"]
    },
    showCurrentDayBorder: true, // Mostrar borde en el día actual (opcional)
    defaultEntryIntensity: 4, // Intensidad predeterminada para las entradas (opcional)
    intensityScaleStart: 10, // Escala de intensidad mínima (opcional)
    intensityScaleEnd: 100, // Escala de intensidad máxima (opcional)
    entries: [] // Lista de entradas para el calendario (se llenará a continuación)
}

// Bucle para llenar las entradas del calendario
for (let page of dv.pages('"daily notes"').where(p => p.exercise)) {
    // Añadir una entrada al calendario para cada página que tenga el campo 'exercise'
    calendarData.entries.push({
        date: page.file.name, // Fecha de la nota (formato YYYY-MM-DD)
        intensity: page.exercise, // Intensidad (valor del campo 'exercise')
        content: "🏋️", // Contenido (emoji de ejercicio, opcional)
        color: "orange" // Color para la entrada (opcional, usa colores definidos arriba)
    });
}

// Renderizar el calendario de mapa de calor
renderHeatmapCalendar(this.container, calendarData);

```