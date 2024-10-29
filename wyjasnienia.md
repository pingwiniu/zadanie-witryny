Podstawy flexow na kartkowke
 
# Podstawy
- Cały kod to tak naprawdę **pudełka z numerkami** (te `div`-y), traktuj je jako kontenery na inne elementy, które mogą mieć swoje atrybuty np wysokość i inne.
- div może zawierać inne elementy i inne divy, elementy w elementach nazywamy dziećmi (child) a elementy w których są rodzicami (parent). Zjawisko to nazywamy **zagnieżdżaniem**. Przykład:

```
<div>  <- parent

    <div>  <- child 
    </div>

</div>

```

# Flex - czyli jak to się układa
- `display: flex` = magiczny sposób na ogarnianie gdzie co ma leżeć
- Masz dwa główne ustawienia w cssie:
  * `flex-direction: row;` = pudełka lecą poziomo (→)
  * `flex-direction: column;` = pudełka lecą pionowo (↓)
- Pamiętaj że zanim ich użyjesz musisz dać `display: flex;` do elementu
 
```markdown
Przykład row (poziomo):
[1][2][3]
 
Przykład column (pionowo):
[1]
[2]
[3]
```
 
# Jak to ogarnąć?
1. Patrz jak pudełka można **zagnieździć** (czyli co jest w czym)
2. Jak zrobisz `row` = rzeczy będą leżeć poziomo
3. Jak zrobisz `column` = rzeczy będą leżeć pionowo
 
# Pro tip
Jak nie ogarniasz co jest gdzie:
Leć od lewej do prawej, patrz co można połączyć żeby stworzyć kwadrat.
<img src="https://i.ibb.co/sgpz5q3/Bez-nazwy.png">
 
Jak coś nie jasne to pisz, pomogę
