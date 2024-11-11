# Zrozumienie Flexboxów

Cześć! Dziś nauczymy się o **Flexboxie** – super narzędziu, które pomaga nam organizować elementy na stronie.

---

## Co to jest Flexbox? 🤔

Flexbox to sposób na ustawienie elementów w rzędzie lub kolumnie na stronie internetowej, dzięki któremu wyglądają schludnie i estetycznie. Wyobraź sobie, że organizujesz swoje biurko, tylko że dla stron internetowych.

---

## Dlaczego warto używać Flexboxa? 📐

Flexbox pozwala:
- Równo rozłożyć elementy na ekranie
- Sterować rozmiarem elementów tak, by dopasowywały się do różnych wielkości ekranów
- Łatwo wyrównywać elementy bez skomplikowanych trików CSS

---

## Kluczowe pojęcia w Flexboxie

Oto kilka słów, które warto znać, pracując z Flexboxem:

1. **Flex Container** 
   - To "pudełko" (zazwyczaj element `div`), które zawiera elementy, które chcemy ułożyć. Kiedy ustawimy `display: flex;` na kontenerze, staje się on Flex Containerm.

2. **Flex Items** 
   - To rzeczy (jak obrazki, przyciski czy tekst) wewnątrz Flex Containera. Flexbox układa te elementy w linii lub stosie.

3. **Rząd** ➡  
   - To linia, wzdłuż której są ustawione elementy. Domyślnie jest **pozioma** (z lewej do prawej), ale można ją zmienić na **pionową** (z góry na dół), jeśli chcesz.

4. **Kolumna** ↕
   - Jest prostopadła do rzędu osi. Czyli góra-dół.

---

## Jak skonfigurować Flexbox

1. **Utwórz kontener**  
   Zacznij od `div` lub innego elementu kontenera:
   ```html
   <div class="flex-container">
       <div class="item">Element 1</div>
       <div class="item">Element 2</div>
       <div class="item">Element 3</div>
   </div>
   ```

2. **Ustaw jako Flex Container**  
   W CSS spraw, by kontener był Flexboxem:
   ```css
   .flex-container {
       display: flex;
   }
   ```

---

## Właściwości Flexbox

### 1. **`flex-direction`**: Wybierz kierunek układu

Ta właściwość decyduje, czy elementy mają iść **z lewej do prawej** (rząd), czy **z góry na dół** (kolumna).

```css
.flex-container {
    flex-direction: row; /* Układ poziomy (domyślny) */
    /* Lub */
    flex-direction: column; /* Układ pionowy */
}
```

### 2. **`justify-content`**: Wyrównaj elementy wzdłuż głównej osi

Użyj tego, aby **rozmieścić elementy** na głównej osi.

- `flex-start`: Elementy zaczynają się od początku
- `center`: Elementy są wyśrodkowane
- `space-between`: Przestrzeń jest dodawana między elementami

```css
.flex-container {
    justify-content: center;
}
```

### 3. **`align-items`**: Wyrównaj elementy na osi krzyżowej

Pomaga wyrównać elementy na osi krzyżowej (na przykład pionowo, jeśli są w rzędzie).

- `flex-start`: Elementy wyrównane do góry
- `center`: Elementy są wyśrodkowane na osi krzyżowej

```css
.flex-container {
    align-items: center;
}
```

---

## Przykład w praktyce 🖥️

Oto przykład układu Flexbox:

```html
<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Przykład Flexbox</title>
    <style>
        .flex-container {
            display: flex;
            flex-direction: row;
            justify-content: space-around;
            align-items: center;
            height: 200px;
            border: 2px solid black;
        }
        .item {
            width: 50px;
            height: 50px;
            background-color: skyblue;
            border: 1px solid navy;
            display: flex;
            justify-content: center;
            align-items: center;
        }
    </style>
</head>
<body>
    <div class="flex-container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
    </div>
</body>
</html>
```

W tym przykładzie:
- Elementy są ułożone w rzędzie.
- Są równomiernie rozmieszczone dzięki `justify-content: space-around`.
- Elementy są wyśrodkowane pionowo.

---

## Wypróbuj sam! 🧪

1. Stwórz plik HTML i skopiuj kod powyżej.
2. Otwórz go w przeglądarce, aby zobaczyć Flexbox w akcji!
3. Spróbuj zmieniać właściwości, takie jak `flex-direction` lub `justify-content`, aby zobaczyć, co się stanie.

---

## Ćwiczenie czyni mistrza 🌟

Eksperymentuj z Flexboxem, aby poczuć się z nim swobodnie! Wkrótce będziesz układać elementy na stronach jak prawdziwy mistrz.

Miłego kodowania! ✨
