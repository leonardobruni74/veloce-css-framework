# 🚀 Veloce CSS Framework v0.1.0-alpha

![Version](https://img.shields.io/badge/version-0.1.0--alpha-orange.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![CSS](https://img.shields.io/badge/100%25-CSS_Puro-orange.svg)

**Veloce** è un framework CSS moderno con documentazione in italiano, creato per chi vuole classi semantiche e intuitive. 100% CSS puro, senza JavaScript, con alta compatibilità browser.

## ✨ Caratteristiche Principali

- ✅ **100% CSS Puro** - Zero dipendenze JavaScript
- ✅ **Naming semantico** - Classi con termini italiani e inglesi, per esempio `sp-btn`, `sp-card` e `sp-grid`
- ✅ **Leggero** - CSS distribuito: circa 56 KiB; non include ancora una versione minificata
- ✅ **Moderno** - Utilizza Flexbox e CSS Grid
- ✅ **Responsive** - Sistema breakpoint integrato
- ✅ **Icone SVG** - Set icone integrate nel CSS
- ✅ **Animazioni CSS** - Effetti senza JavaScript
- ✅ **Alta Compatibilità** - Pensato per browser moderni; verifica la compatibilità richiesta dal tuo progetto
- ✅ **Personalizzabile** - CSS Variables per facile customizzazione

## 📦 Installazione

### Download Diretto

Scarica i file `fast.css` e includilo nella pagina HTML:

```html
<!DOCTYPE html>
<html lang="it">
<head>
  <link rel="stylesheet" href="fast.css">
</head>
<body>
  <!-- Il tuo contenuto -->
</body>
</html>
```

## 🎨 Palette Colori

Veloce include una palette di colori completa:

### Colori Primari
- `--color-primary`: #0066cc
- `--color-secondary`: #ff6b35
- `--color-success`: #2ecc71
- `--color-danger`: #e74c3c
- `--color-info`: #9b59b6
- `--color-pink`: #ff4081
- `--color-warning`: #f1c40f

### Scala Grigi
- `--color-black`: #1a1a1a
- `--color-gray-dark`: #2c3e50
- `--color-gray`: #7f8c8d
- `--color-gray-light`: #bdc3c7
- `--color-gray-lighter`: #ecf0f1
- `--color-white`: #ffffff

## 📖 Guida Rapida

### Layout con Grid System

```html
<!-- Grid Base -->
<div class="sp-grid sp-grid-3 sp-gap-md">
  <div>Colonna 1</div>
  <div>Colonna 2</div>
  <div>Colonna 3</div>
</div>

<!-- Grid Responsive -->
<div class="sp-grid sp-grid-1 sp-md:grid-3 sp-lg:grid-4 sp-gap-lg">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
  <div>Item 4</div>
</div>

<!-- Column Span -->
<div class="sp-grid sp-grid-4 sp-gap-md">
  <div class="sp-col-span-2">Span 2 colonne</div>
  <div>Item</div>
  <div>Item</div>
</div>
```

### Flexbox System

```html
<!-- Flex Center -->
<div class="sp-flex sp-justify-center sp-items-center sp-gap-md">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
</div>

<!-- Flex Between -->
<div class="sp-flex sp-justify-between sp-items-center">
  <div>Sinistra</div>
  <div>Centro</div>
  <div>Destra</div>
</div>

<!-- Flex Column -->
<div class="sp-flex sp-flex-col sp-gap-sm">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
</div>
```

### Bottoni

```html
<!-- Bottoni Colorati -->
<button class="sp-btn sp-btn-primary">Azzurro</button>
<button class="sp-btn sp-btn-secondary">Arancio</button>
<button class="sp-btn sp-btn-success">Verde</button>
<button class="sp-btn sp-btn-danger">Rosso</button>

<!-- Bottoni Outline -->
<button class="sp-btn sp-btn-outline">Outline Azzurro</button>
<button class="sp-btn sp-btn-outline-success">Outline Verde</button>

<!-- Dimensioni -->
<button class="sp-btn sp-btn-primary sp-btn-sm">Piccolo</button>
<button class="sp-btn sp-btn-primary">Normale</button>
<button class="sp-btn sp-btn-primary sp-btn-lg">Grande</button>
<button class="sp-btn sp-btn-primary sp-btn-xl">Enorme</button>

<!-- Bottone Blocco -->
<button class="sp-btn sp-btn-primary sp-btn-block">100% Larghezza</button>
```

### Carte (Cards)

```html
<!-- Carta Base -->
<div class="sp-card">
  <h3 class="sp-card-title">Titolo Carta</h3>
  <p>Contenuto della card con effetto hover automatico.</p>
  <button class="sp-btn sp-btn-primary sp-mt-md">Azione</button>
</div>

<!-- Carta Colorata -->
<div class="sp-card sp-card-primary">
  <h3 class="sp-card-title">Carta Azzurra</h3>
  <p>Questa card ha sfondo azzurro e testo bianco.</p>
</div>

<!-- Carta con Struttura -->
<div class="sp-card">
  <div class="sp-card-header">
    <h4 class="sp-card-title">Intestazione</h4>
  </div>
  <div class="sp-card-body">
    <p>Corpo della card</p>
  </div>
  <div class="sp-card-footer">
    <button class="sp-btn sp-btn-primary">OK</button>
  </div>
</div>
```

### Badge

```html
<span class="sp-badge sp-badge-primary">Azzurro</span>
<span class="sp-badge sp-badge-success">Successo</span>
<span class="sp-badge sp-badge-danger">Errore</span>
<span class="sp-badge sp-badge-outline">Outline</span>

<!-- Uso pratico -->
<p>Notifiche <span class="sp-badge sp-badge-danger">5</span></p>
<p>Stato: <span class="sp-badge sp-badge-success">Attivo</span></p>
```

### Avvisi

```html
<div class="sp-alert sp-alert-success">
  <div class="sp-alert-title">Operazione Completata!</div>
  <p>I tuoi dati sono stati salvati.</p>
</div>

<div class="sp-alert sp-alert-info">
  <div class="sp-alert-title">Informazione</div>
  <p>Notifica informativa.</p>
</div>

<div class="sp-alert sp-alert-warning">
  <div class="sp-alert-title">Attenzione</div>
  <p>Verifica i dati prima di procedere.</p>
</div>

<div class="sp-alert sp-alert-danger">
  <div class="sp-alert-title">Errore</div>
  <p>Si è verificato un errore.</p>
</div>
```

### Moduli (Forms)

```html
<form>
  <div class="sp-form-group">
    <label class="sp-form-label" for="nome">Nome</label>
    <input id="nome" type="text" class="sp-form-control" placeholder="Inserisci nome">
  </div>

  <div class="sp-form-group">
    <label class="sp-form-label" for="email">Email</label>
    <input id="email" type="email" class="sp-form-control" placeholder="email@esempio.com">
    <span class="sp-form-help">Messaggio di aiuto</span>
  </div>

  <div class="sp-form-group">
    <label class="sp-form-label" for="paese">Paese</label>
    <select id="paese" class="sp-form-control">
      <option>Italia</option>
      <option>Francia</option>
      <option>Germania</option>
    </select>
  </div>

  <div class="sp-form-group">
    <label class="sp-form-label" for="messaggio">Messaggio</label>
    <textarea id="messaggio" class="sp-form-control" placeholder="Il tuo messaggio"></textarea>
  </div>

  <div class="sp-form-group">
    <label class="sp-form-check-label">
      <input type="checkbox" class="sp-form-check">
      <span>Accetto i termini</span>
    </label>
  </div>

  <button type="submit" class="sp-btn sp-btn-primary">Invia</button>
</form>
```

### Tabelle

```html
<!-- Tabella Base -->
<table class="sp-table">
  <thead>
    <tr>
      <th>Nome</th>
      <th>Email</th>
      <th>Ruolo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Mario Rossi</td>
      <td>mario@example.com</td>
      <td>Admin</td>
    </tr>
    <tr>
      <td>Giulia Bianchi</td>
      <td>giulia@example.com</td>
      <td>Editor</td>
    </tr>
  </tbody>
</table>

<!-- Tabella Striata -->
<table class="sp-table sp-table-striped">
  <!-- contenuto -->
</table>

<!-- Tabella Bordata -->
<table class="sp-table sp-table-bordered">
  <!-- contenuto -->
</table>
```

### Navigazione

```html
<!-- Navbar -->
<nav class="sp-navbar">
  <a href="#" class="sp-navbar-brand">Brand</a>
  <ul class="sp-navbar-menu">
    <li><a href="#" class="sp-navbar-link">Home</a></li>
    <li><a href="#" class="sp-navbar-link">Prodotti</a></li>
    <li><a href="#" class="sp-navbar-link">Contatti</a></li>
  </ul>
</nav>

<!-- Breadcrumb -->
<ul class="sp-breadcrumb">
  <li class="sp-breadcrumb-item"><a href="#" class="sp-breadcrumb-link">Home</a></li>
  <li class="sp-breadcrumb-item"><a href="#" class="sp-breadcrumb-link">Prodotti</a></li>
  <li class="sp-breadcrumb-item sp-active">Laptop</li>
</ul>

<!-- Paginazione -->
<ul class="sp-pagination">
  <li class="sp-pagination-item"><a href="#" class="sp-pagination-link">‹</a></li>
  <li class="sp-pagination-item sp-active"><a href="#" class="sp-pagination-link">1</a></li>
  <li class="sp-pagination-item"><a href="#" class="sp-pagination-link">2</a></li>
  <li class="sp-pagination-item"><a href="#" class="sp-pagination-link">3</a></li>
  <li class="sp-pagination-item"><a href="#" class="sp-pagination-link">›</a></li>
</ul>
```

### Progress Bar

```html
<!-- Barra Base -->
<div class="sp-progress">
  <div class="sp-progress-bar" style="width: 75%;">75%</div>
</div>

<!-- Barra Colorata -->
<div class="sp-progress sp-progress-success">
  <div class="sp-progress-bar" style="width: 60%;">60%</div>
</div>

<!-- Barra Animata -->
<div class="sp-progress sp-progress-striped">
  <div class="sp-progress-bar" style="width: 50%;"></div>
</div>
```

### Spinner

```html
<!-- Spinner Base -->
<div class="sp-spinner"></div>

<!-- Dimensioni -->
<div class="sp-spinner sp-spinner-sm"></div>
<div class="sp-spinner"></div>
<div class="sp-spinner sp-spinner-lg"></div>

<!-- Colori -->
<div class="sp-spinner sp-spinner-secondary"></div>
<div class="sp-spinner sp-spinner-success"></div>
```

### Icone SVG

```html
<!-- Icone integrate nel CSS -->
<span class="sp-icon sp-icon-home sp-text-primary"></span>
<span class="sp-icon sp-icon-user sp-text-primary"></span>
<span class="sp-icon sp-icon-email sp-text-primary"></span>
<span class="sp-icon sp-icon-settings sp-text-primary"></span>
<span class="sp-icon sp-icon-search sp-text-primary"></span>
<span class="sp-icon sp-icon-menu sp-text-primary"></span>
<span class="sp-icon sp-icon-close sp-text-danger"></span>
<span class="sp-icon sp-icon-heart sp-text-danger"></span>
<span class="sp-icon sp-icon-star sp-text-warning"></span>
<span class="sp-icon sp-icon-check sp-text-success"></span>
<span class="sp-icon sp-icon-info sp-text-primary"></span>
<span class="sp-icon sp-icon-warning sp-text-secondary"></span>
<span class="sp-icon sp-icon-cart sp-text-info"></span>
<span class="sp-icon sp-icon-download sp-text-success"></span>

<!-- Dimensioni -->
<span class="sp-icon sp-icon-sm sp-icon-home"></span>
<span class="sp-icon sp-icon-home"></span>
<span class="sp-icon sp-icon-md sp-icon-home"></span>
<span class="sp-icon sp-icon-lg sp-icon-home"></span>
```

## 🎬 Animazioni CSS

Tutte le animazioni sono in CSS puro, senza JavaScript:

```html
<!-- Animazioni di Entrata -->
<div class="sp-animate-fade-in">Fade In</div>
<div class="sp-animate-slide-up">Slide Up</div>
<div class="sp-animate-slide-down">Slide Down</div>
<div class="sp-animate-scale-in">Scale In</div>

<!-- Animazioni Continue -->
<div class="sp-animate-pulse">Pulsazione continua</div>
<div class="sp-animate-bounce">Effetto rimbalzo</div>
<div class="sp-animate-shake">Effetto shake</div>

<!-- Effetti Hover -->
<div class="sp-hover-lift">Solleva al hover</div>
<div class="sp-hover-grow">Cresce al hover</div>
<div class="sp-hover-rotate">Ruota al hover</div>
```

## 📱 Responsive Design

Veloce usa un sistema mobile-first con breakpoint standard:

- `sp-sm:` - min-width: 640px (tablet piccoli)
- `sp-md:` - min-width: 768px (tablet)
- `sp-lg:` - min-width: 1024px (desktop)
- `sp-xl:` - min-width: 1280px (desktop large)

```html
<!-- Grid Responsive -->
<div class="sp-grid sp-grid-1 sp-sm:grid-2 sp-md:grid-3 sp-lg:grid-4">
  <!-- Si adatta automaticamente -->
</div>

<!-- Flex Responsive -->
<div class="sp-flex sp-flex-col sp-md:flex-row">
  <!-- Colonna su mobile, riga su desktop -->
</div>

<!-- Visibilità Responsive -->
<div class="sp-hidden sp-md:block">Visibile solo su desktop</div>
<div class="sp-block sp-md:hidden">Visibile solo su mobile</div>
```

### Orientamento e TV

```html
<!-- Solo in verticale/orizzontale -->
<div class="sp-portrait:block sp-landscape:hidden">Solo Portrait</div>
<div class="sp-portrait:hidden sp-landscape:block">Solo Landscape</div>

<!-- TV / Schermi grandi -->
<div class="sp-grid sp-grid-2 sp-tv:grid-6">...</div>
```

## 🎨 Personalizzazione

Puoi facilmente personalizzare Veloce sovrascrivendo le CSS Variables:

```css
:root {
  /* Personalizza i colori */
  --color-primary: #007bff;
  --color-secondary: #fd7e14;
  
  /* Personalizza le spaziature */
  --spacing-md: 1.2rem;
  
  /* Personalizza le ombre */
  --shadow-md: 0 6px 12px rgba(0, 0, 0, 0.15);
  
  /* Personalizza i font */
  --font-base: 'Helvetica', sans-serif;
}
```

## 🔧 Utility Classes

### Spaziatura

```html
<!-- Margini -->
<div class="sp-m-xs">Margine extra small</div>
<div class="sp-m-md">Margine medio</div>
<div class="sp-mx-auto">Margine auto orizzontale (centra)</div>
<div class="sp-mt-lg">Margine solo sopra</div>

<!-- Padding -->
<div class="sp-p-sm">Padding small</div>
<div class="sp-p-lg">Padding large</div>
<div class="sp-px-md">Padding orizzontale</div>
<div class="sp-py-xl">Padding verticale</div>
```

### Tipografia

```html
<!-- Dimensioni -->
<p class="sp-text-xs">Testo extra small</p>
<p class="sp-text-2xl">Testo 2XL</p>
<p class="sp-text-5xl">Testo 5XL</p>

<!-- Peso -->
<p class="sp-font-light">Font leggero</p>
<p class="sp-font-bold">Font grassetto</p>

<!-- Allineamento -->
<p class="sp-text-left">Allineato a sinistra</p>
<p class="sp-text-center">Centrato</p>
<p class="sp-text-right">Allineato a destra</p>

<!-- Trasformazione -->
<p class="sp-uppercase">tutto uppercase</p>
<p class="sp-capitalize">prima lettera maiuscola</p>
```

### Colori

```html
<!-- Testo -->
<p class="sp-text-primary">Testo azzurro</p>
<p class="sp-text-success">Testo verde</p>
<p class="sp-text-danger">Testo rosso</p>

<!-- Sfondo -->
<div class="sp-bg-primary sp-text-white">Sfondo azzurro</div>
<div class="sp-bg-gray-lighter">Sfondo grigio pallido</div>

<!-- Gradienti -->
<div class="sp-gradient-primary sp-text-white">Gradiente azzurro</div>
<div class="sp-gradient-sunset sp-text-white">Gradiente tramonto</div>
```

### Display e Posizionamento

```html
<!-- Display -->
<div class="sp-hidden">Nascosto</div>
<div class="sp-block">Blocco</div>
<div class="sp-inline-block">Inline block</div>

<!-- Posizionamento -->
<div class="sp-relative">Posizione relativa</div>
<div class="sp-absolute">Posizione assoluta</div>
<div class="sp-fixed">Posizione fissa</div>

<!-- Larghezza/Altezza -->
<div class="sp-w-full">100% larghezza</div>
<div class="sp-h-screen-100">100vh altezza</div>
```

### Bordi e Ombre

```html
<!-- Bordi -->
<div class="sp-border">Bordo base</div>
<div class="sp-border-t">Bordo solo sopra</div>

<!-- Arrotondamenti -->
<div class="sp-rounded-sm">Arrotondato piccolo</div>
<div class="sp-rounded-lg">Arrotondato grande</div>
<div class="sp-rounded-full">Completamente arrotondato</div>

<!-- Ombre -->
<div class="sp-shadow-sm">Ombra piccola</div>
<div class="sp-shadow-md">Ombra media</div>
<div class="sp-shadow-lg">Ombra grande</div>
```

## 📋 Esempi Completi

### Login Form

```html
<div class="sp-container-sm sp-py-3xl">
  <div class="sp-card">
    <h2 class="sp-h2 sp-text-center sp-mb-lg">Accedi</h2>
    
    <form>
      <div class="sp-form-group">
        <label class="sp-form-label" for="email">Email</label>
        <input id="email" type="email" class="sp-form-control" placeholder="email@esempio.com">
      </div>
      
      <div class="sp-form-group">
        <label class="sp-form-label" for="password">Password</label>
        <input id="password" type="password" class="sp-form-control" placeholder="••••••••">
      </div>
      
      <div class="sp-form-group">
        <label class="sp-form-check-label">
          <input type="checkbox" class="sp-form-check">
          <span>Ricordami</span>
        </label>
      </div>
      
      <button type="submit" class="sp-btn sp-btn-primary sp-btn-block sp-mb-md">
        Accedi
      </button>
      
      <p class="sp-text-center sp-text-sm sp-text-gray">
        Non hai un account? <a href="#" class="sp-text-primary">Registrati</a>
      </p>
    </form>
  </div>
</div>
```

### Dashboard Cards

```html
<div class="sp-container sp-py-xl">
  <h1 class="sp-h1 sp-mb-lg">Dashboard</h1>
  
  <div class="sp-grid sp-grid-1 sp-md:grid-4 sp-gap-lg sp-mb-xl">
    <div class="sp-card sp-bg-primary sp-text-white">
      <p class="sp-text-sm sp-mb-xs">Totale Vendite</p>
      <p class="sp-text-4xl sp-font-bold">€12,345</p>
      <p class="sp-text-sm" style="opacity: 0.8;">+12% dal mese scorso</p>
    </div>
    
    <div class="sp-card sp-bg-success sp-text-white">
      <p class="sp-text-sm sp-mb-xs">Nuovi Clienti</p>
      <p class="sp-text-4xl sp-font-bold">234</p>
      <p class="sp-text-sm" style="opacity: 0.8;">+5% questa settimana</p>
    </div>
    
    <div class="sp-card sp-bg-secondary sp-text-white">
      <p class="sp-text-sm sp-mb-xs">Ordini Pending</p>
      <p class="sp-text-4xl sp-font-bold">18</p>
      <p class="sp-text-sm" style="opacity: 0.8;">Da processare</p>
    </div>
    
    <div class="sp-card sp-bg-info sp-text-white">
      <p class="sp-text-sm sp-mb-xs">Prodotti</p>
      <p class="sp-text-4xl sp-font-bold">567</p>
      <p class="sp-text-sm" style="opacity: 0.8;">Nel catalogo</p>
    </div>
  </div>
  
  <!-- Tabella recenti ordini -->
  <div class="sp-card">
    <h3 class="sp-h3 sp-mb-md">Ordini Recenti</h3>
    <table class="sp-table">
      <thead>
        <tr>
          <th>#</th>
          <th>Cliente</th>
          <th>Prodotto</th>
          <th>Importo</th>
          <th>Stato</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>1001</td>
          <td>Mario Rossi</td>
          <td>Laptop Pro</td>
          <td>€1,299</td>
          <td><span class="sp-badge sp-badge-success">Completato</span></td>
        </tr>
        <tr>
          <td>1002</td>
          <td>Giulia Bianchi</td>
          <td>Monitor 4K</td>
          <td>€499</td>
          <td><span class="sp-badge sp-badge-secondary">In elaborazione</span></td>
        </tr>
        <tr>
          <td>1003</td>
          <td>Luca Verdi</td>
          <td>Mouse Wireless</td>
          <td>€49</td>
          <td><span class="sp-badge sp-badge-success">Completato</span></td>
        </tr>
      </tbody>
    </table>
  </div>
</div>
```

## 🌐 Compatibilità Browser

Veloce è compatibile con:
- ✅ Chrome (ultime 2 versioni)
- ✅ Firefox (ultime 2 versioni)
- ✅ Safari (ultime 2 versioni)
- ✅ Edge (ultime 2 versioni)
- ✅ Opera (ultime 2 versioni)

## 📄 Licenza

MIT License - Libero per uso personale e commerciale.

## 🤝 Contributi

I contributi sono benvenuti! Se vuoi contribuire:
1. Fork del repository
2. Crea un branch per la tua feature
3. Commit delle modifiche
4. Push al branch
5. Apri una Pull Request

## 📞 Supporto

- 📖 Documentazione: Vedi `demo.html` per esempi completi
- 💬 Community: da definire
- 🐛 Bug report: usa la sezione Issues del repository

---

**Creato con ❤️ per la comunità italiana di sviluppatori web**

*Veloce - Il framework CSS che parla italiano*

