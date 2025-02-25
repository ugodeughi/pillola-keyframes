# 🚀 Animazioni fluide con @keyframes e animation

Le **animazioni CSS** permettono di creare effetti dinamici senza JavaScript, migliorando l'interattività del sito.

## 🎬 Come funzionano le animazioni CSS?
CSS offre la possibilità di creare effetti di movimento grazie a due strumenti fondamentali:

1️⃣ **`@keyframes`** → Definisce le fasi dell'animazione  
2️⃣ **`animation`** → Applica l'animazione a un elemento con opzioni personalizzabili  

📌 **Opzioni principali di `animation`:**
- `animation-duration` → Durata dell'animazione  
- `animation-timing-function` → Tipo di accelerazione (`ease`, `linear`, `ease-in`, etc.)  
- `animation-iteration-count` → Numero di ripetizioni (es. `infinite`)  
- `animation-delay` → Ritardo prima dell'inizio  
- `animation-direction` → Direzione (`normal`, `reverse`, `alternate`)  

---

## 🛠️ Esempio 1: Bottone che pulsa 🔵
### **Effetto:** Il pulsante si ingrandisce e rimpicciolisce automaticamente.  

### ✅ **HTML**
```html
<button class="btn-animated">Cliccami!</button>
```

### 🎨 **CSS**
```css
@keyframes pulse {
  0% { transform: scale(1); }
  50% { transform: scale(1.1); }
  100% { transform: scale(1); }
}

.btn-animated {
  background-color: #007bff;
  color: white;
  padding: 10px 20px;
  border: none;
  font-size: 18px;
  cursor: pointer;
  animation: pulse 1.5s infinite ease-in-out;
}
```

**🔹 Cosa fa?**  
✔️ Ogni 1.5 secondi il bottone aumenta di dimensione del **10%**  
✔️ L'effetto è **fluido** grazie alla funzione `ease-in-out`  
✔️ L'animazione è **infinita**  

---

## 🌀 Esempio 2: Loading Spinner 🔄
### **Effetto:** Un cerchio ruota simulando un caricamento.  

### ✅ **HTML**
```html
<div class="loader"></div>
```

### 🎨 **CSS**
```css
@keyframes spin {
  0% { transform: rotate(0deg); }
  100% { transform: rotate(360deg); }
}

.loader {
  width: 50px;
  height: 50px;
  border: 5px solid #ccc;
  border-top: 5px solid #007bff;
  border-radius: 50%;
  animation: spin 1s linear infinite;
}
```

**🔹 Cosa fa?**  
✔️ Il cerchio ruota di **360°** in **1 secondo**  
✔️ L'animazione è **continua e fluida**  
✔️ Perfetto per **loading screens e attese utente**  

---

## 🔥 Altri effetti animati con CSS
💡 Puoi combinare `@keyframes` con altre proprietà CSS per creare animazioni più avanzate:  
🔹 **Effetti di fade-in/fade-out** con `opacity`  
🔹 **Animazioni di rimbalzo** con `cubic-bezier`  
🔹 **Testi che scorrono** con `transform: translateX()`  

---

## 🌍 Browser Support
🔹 **Chrome, Edge, Firefox, Safari, Opera** → Supportano le animazioni CSS dalla versione 5+ 🚀  
🔹 **Internet Explorer 9+** → Richiede `-webkit-` per compatibilità  

---

## 📌 Conclusione
Le **animazioni CSS** sono un potente strumento per migliorare l'esperienza utente **senza JavaScript**!  

🚀 **Hai provato a usarle nei tuoi progetti?**  

🔖 #CSS #WebDevelopment #Animations #PilloleDiWebDev #UgoDeUghi
