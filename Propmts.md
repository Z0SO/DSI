
```markdown
Hola necesito que te dediques a hacer apuntes para estudiar sobre la materia DISEÑO DE SISTEMAS que sean hermosisimos en markdown para obsidian, te voy a pasar los textos de mis apuntes en docs y tu procesaras todo como te dije. vas a hacer siempre eso a menos que te indique lo contrario
```


```dataviewjs
// PS. elimina la barra invertida \ al principio! 
dv.span("** 😊 Título 😥**") /* opcional ⏹️💤⚡⚠🧩↑↓⏳📔💾📁📝🔄📝🔀⌨️🕸️📅🔍✨ */

// Configuración del calendario
const calendarData = { 
    year: 2022, // (opcional) por defecto, el año actual
    colors: { // (opcional) por defecto, verde
        blue: ["#8cb9ff", "#69a3ff", "#428bff", "#1872ff", "#0058e2"], // la primera entrada se considera la predeterminada si se suministra
        green: ["#c6e48b", "#7bc96f", "#49af5d", "#2e8840", "#196127"],
        red: ["#ff9e82", "#ff7b55", "#ff4d1a", "#e73400", "#bd2a00"],
        orange: ["#ffa244", "#fd7f00", "#dd6f00", "#bf6000", "#9b4e00"],
        pink: ["#ff96cb", "#ff70b8", "#ff3a9d", "#ee0077", "#c30062"],
        orangeToRed: ["#ffdf04", "#ffbe04", "#ff9a03", "#ff6d02", "#ff2c01"]
    },
    showCurrentDayBorder: true, // (opcional) por defecto, true
    defaultEntryIntensity: 4, // (opcional) por defecto, 4
    intensityScaleStart: 10, // (opcional) por defecto, el valor más bajo pasado a entries.intensity
    intensityScaleEnd: 100, // (opcional) por defecto, el valor más alto pasado a entries.intensity
    entries: [] // (obligatorio) se llena en el bucle DataviewJS a continuación
}

// Bucle DataviewJS para llenar las entradas del calendario
for (let page of dv.pages('"daily notes"').where(p => p.exercise)) {
    calendarData.entries.push({
        date: page.file.name, // (obligatorio) Formato YYYY-MM-DD
        intensity: page.exercise, // (obligatorio) los datos que deseas rastrear, mapeará las intensidades de color automáticamente
        content: "🏋️", // (opcional) Añadir texto a la celda de la fecha
        color: "orange" // (opcional) Referencia de *calendarData.colors*. Si no se suministra color, se usa colors[0]
    });
}

// Renderizar el calendario de mapa de calor
renderHeatmapCalendar(this.container, calendarData);

```