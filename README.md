# Container Queries: CSS responsive senza media queries

## 🔹 Introduzione
Le **Container Queries** permettono di adattare il layout di un componente in base alle dimensioni del suo **contenitore**, anziché in base al **viewport**. Questo le rende un'ottima alternativa alle media queries tradizionali.

## 📌 Come funzionano?
Per attivare le container queries, si usa `container-type: inline-size;` all'interno del CSS del contenitore. In questo modo, gli stili vengono applicati in base alla larghezza del contenitore stesso.

### 🛠️ **Esempio pratico**

```css
/* Definizione del contenitore */
.card-container {
  container-type: inline-size; /* Attiva le container queries */
  max-width: 600px;
  border: 2px solid #333;
  padding: 16px;
  margin: 20px auto;
  background-color: #f8f8f8;
}

/* Stili base della card */
.card {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  background: white;
  padding: 16px;
  border-radius: 8px;
  box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.1);
}

.card img {
  width: 100%;
  max-width: 200px;
  border-radius: 8px;
}

.card h3 {
  margin: 12px 0;
  color: brown;
}

/* Stili condizionali basati sulla larghezza del contenitore */
@container (min-width: 500px) {
  .card {
    flex-direction: row;
    text-align: left;
  }

  .card img {
    width: 100px;
    margin-right: 16px;
  }

  .card h3 {
    color: cadetblue;
  }
}
```

## ✅ **Perché usare le Container Queries?**
- 📌 **Componenti veramente riutilizzabili** 🎯
- 🧹 **CSS più pulito e scalabile**
- 🚀 **Responsive design senza media queries globali**

## 🔗 **Compatibilità browser**
Le Container Queries sono supportate nei browser moderni (Chrome, Edge, Firefox, Safari). Controlla il supporto su [Can I Use](https://caniuse.com/css-container-queries).

---
🔥 **Ti sembra utile? Condividi e sperimenta nei tuoi progetti!** 🚀
