Rozumiem, chcesz rozbudować kod. W takim razie możemy dodać kilka funkcji, takich jak nowe ataki, różnorodność przeciwników, czy system nagród. Poniżej przedstawiam rozwinięty kod:

```python
import random

# ... (poprzednia część kodu)

# Nowe ataki gracza
dmggracza4 = [[25, 35], [35, 45], [40, 50], [50, 60], [60, 70], [70, 80], [80, 90], [90, 100]]

# Nowe przeciwnicy
nazwyprzeciwnikow += ["joker", "venom", "thanos"]
hpprzeciwnikow += [[120, [50, 100]], [200, [30, 60]], [300, [80, 150]]]

# Nowe poziomy ulepszeń
koszt += [250, 350, 450, 600, 800, 1000, 1500]

# System nagród za pokonanie przeciwnika
nagrody = [100, 150, 200, 300, 500]

# ... (poprzednia część kodu)

def print_nagrody():
    print("Nagrody za pokonanie przeciwników:")
    for i, nagroda in enumerate(nagrody, start=1):
        print(f"{i} - {nagroda} pieniędzy")

# ... (poprzednia część kodu)

def walka(nazwa_przeciwnika, zakres_hp_przeciwnika):
    # ... (poprzednia część kodu)

    if twoje_hp > 0:
        nagroda_index = pokonani.count(0) - 1
        nagroda = nagrody[nagroda_index] if nagroda_index < len(nagrody) else nagrody[-1]
        pieniadze += nagroda
        print(f"Wygrałeś!\nOtrzymujesz {nagroda} pieniędzy!")
        return True
    else:
        print("Przegrałeś!")
        return False

# ... (poprzednia część kodu)

def lobby():
    # ... (poprzednia część kodu)
    print("N - Nagrody za pokonanie przeciwników")
    # ... (poprzednia część kodu)
    return input("Wybierz Akcję: ")

# ... (poprzednia część kodu)

if __name__ == "__main__":
    # ... (poprzednia część kodu)
    while dziala:
        akcja = lobby()

        if akcja.isdigit() and 1 <= int(akcja) <= 8:
            # ... (poprzednia część kodu)
        elif akcja == "N":
            print_nagrody()
        # ... (poprzednia część kodu)
```

Wprowadziłem nowe ataki, przeciwników, poziomy ulepszeń, system nagród za pokonanie przeciwników, oraz odpowiednie modyfikacje w funkcji `walka` i `lobby`. Oczywiście, możemy nadal dodawać nowe elementy i r
ozwijać grę według potrzeb.
