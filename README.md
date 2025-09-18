# mapa-aaccaparica
Mapa interativo para visualização de praias intervencionadas em almada

# 🗺️ Mapa Interativo – Intervenção Cova-Gala / Lavos

Este repositório contém o ficheiro `index.html` com o mapa interativo desenvolvido em Leaflet.js. O mapa apresenta os diferentes troços de praia afetados pela intervenção costeira, com cores distintas consoante o estado de cada fase.

---

##  Como atualizar o estado das praias

### 1. Abrir o ficheiro `index.html` num editor de texto (ex.: VSCode, Sublime Text ou mesmo Notepad++)

### 2. Localizar o bloco correspondente à fase/praia a atualizar
Exemplo:

```js
L.polygon([
  [40.127892419955536, -8.864797353744509],
  [40.127662725736414, -8.863445520401003],
  [40.126079455183955, -8.86402487754822],
  [40.126276340576446, -8.865290880203249]
], {
  color: "red",
  fillColor: "red",
  fillOpacity: 0.5
}).addTo(map).bindPopup("<h3>Fase 1</h3><strong>Estado Atual:</strong> Em Intervenção (Interdita)<br><strong>Fim Intervenção:</strong> julho 2025");
```

---

##  O que pode ser alterado

### COR (estado da intervenção):

- `"red"` = Em Intervenção (Interdita)
- `"orange"` = Intervenção Planeada (Permitida)
- `"green"` = Intervenção Concluída (Permitida)

Modificar nos campos:
```js
color: "red",
fillColor: "red"
```

---

### TEXTO (popup da praia):

Modificar a seguinte string:
```html
<h3>Fase 1</h3>
<strong>Estado Atual:</strong> Em Intervenção (Interdita)<br>
<strong>Fim Intervenção:</strong> julho 2025
```

Pode alterar:
- o nome da fase/praia (`Fase 1`)
- o estado atual (ex.: `Em Intervenção (Interdita)`, `Intervenção Concluída (Permitida)`)
- a data prevista de fim/intervenção

---


Dúvidas: pedropimentel@unimagem.pt 
