# Interactive rating component solution

## Overview

Users should be able to:

- View the optimal layout for the app depending on their device's screen size
- See hover states for all interactive elements on the page
- Select and submit a number rating
- See the "Thank you" card state after submitting a rating

### Screenshot

**Snapshot of `Rating card` at desktop width 1440px**

![](images/Interactive-snap-1.png)

**Snapshot of `Thank you card` at desktop width 1440px**

![](images/Interactive-snap-2.png)

### Built with

- Vanilla JavaScript
- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### Concepts Used

- Use **data-value** to get rating value

```JS
const ratingGet = num.getAttribute('data-value');
```

- Use **session-storage** to store rating value temporary to show it in another page

```JS
sessionStorage.setItem('ratingGet', ratingGet);
```

Also to retrieve rating value

```JS
const ratingValue = sessionStorage.getItem('ratingGet');
```

- Use **window.location.href** to move at another page

```JS
window.location.href = 'index2.html';
```

- Use **template literals** to show selected rating

```JS
rating.innerHTML = `You selected ${ratingValue} out of 5`;
```

## Author

Meenu Soni 👨‍💻
