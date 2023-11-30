from random import randint
print("podaj imie bohatera")
name = input()
print ("witaj " + name) 

life = 100 
mana = 200 
money = 700

print(f"Masz {life} HP  {mana} many i {money} pięniędzy ")

print("Aby zagrać wybierz poziom trudności")

print ("--1. łatwy--")
print ("--2. Normalny--")
print("--3. Trudny--")

trudność = input("Wybierz poziom trudności ")

if trudność == '1':
    print("wybrałeś poziom łatwy kliknj 1 aby rozpocząć rozgrywke")
    życia = 3
elif trudność == "2":
    print("wybrałeś poziom Normalny kliknj 2 aby rozpocząć rozgrywke")
    życia = 2
elif trudność == "3":
    życia = 1
    print("wybrałeś poziom Trudny kliknj 3 aby rozpocząć rozgrywke")


gra = input("Omówienie ")
if gra == "1":
    print("Witaj aby wygrać musisz dokonywać własciwych wyborów jeśli wybierzesz źle tracisz życie na poziomie łatwtym masz 2 życia będziessz miał/a do wyboru od 2 do 4 opcji jeśli wybierzesz tracisz hp ")
if gra == "2":
    print("Witaj aby wygrać musisz dokonywać własciwych wyborów jeśli wybierzesz źle tracisz życie na poziomie Normalnym masz 2 życia będziessz miał/a do wyboru od 2 do 4 opcji jeśli wybierzesz tracisz hp ")
if gra == "3":
    print("Witaj aby wygrać musisz dokonywać własciwych wyborów jeśli wybierzesz źle tracisz życie na poziomie Trudnym masz 1 życia będziessz miał/a do wyboru od 2 do 4 opcji jeśli wybierzesz tracisz hp  ")


print (" kliknij 1 aby zapoznać się z fabułą gry")

start = input("Wprowadzenie faburalne")

if start == "1":
    print("W magicznym królestwie, bohater wyrusza na wyprawę, by pokonać mroczne potwory zwiastujące nadejście chaosu. Musi odkryć zaklęcia i odnaleźć legendarną broń, by uratować świat przed zgubą.")



print(name  + "jesteś podczas konnej wyprawy, atakuje cie zmutowany wilk oto twoje opcje ")
print("-1- walczysz z wikiem")
print("-2- jedziesz inną drogą")
print("-3- omijasz go jadąc przez las")

decyzja = input("podejmij decyzje ")

if decyzja == "1":
    print("wygrałeś i sprzedałeś skóre wilka  masz teraz ")
    life -= 16
    mana -= 30
    money += 120

elif decyzja =="2":
    print("spotykasz na innej drodze bandytów którzy ukradli ci 200 monet ale poobijany i zmęczony uciekłeś")
    life -= 24
    mana -= 70
    money -= 200

elif  decyzja =="3":
    print("w lesie znajdujesz worek z mnetami ale kaleczysz się o ciernie więc tracisz hp")
    life -= 10
    money += 150

print(f"Masz {life} HP  {mana} many i {money} pięniędzy ")

print( name  + " przejerzdżasz obok wioski (muszisz jechać do sklepu)")
print("-1- jedziesz do sklepu")
decyzja = input("zdecyduj się")
if decyzja == "1":
    print("możesz kupić następujące towary")
    
    print("--1. woda")
    print("--2. chleb")
    print("--3. jabłko")
    print("--4. mikstura_zdrowia")
    print("--5. mikstura_siły")
    print("--6. tarcza")
    print("--7. zbroja")
    print("--8. mityczna broń której potrzebujesz aby pokonać mroczne potwory")
    print("możesz  kupić tylko 1 rzecz")

    zakupy = input("wybierz co chesz kupić")

    if zakupy == "1":
     life+=8   
     money-=10

    if zakupy == "2":
     life+=11  
     money-=13

    if zakupy == "3":
     life+=9  
     money-=7

    if zakupy == "4":
     life+=20  
     money-=30

    if zakupy == "5":
     mana+=30 
     money-=40

    if zakupy == "6":
     life+= 40 
     money-=100

    if zakupy == "7":
     life+= 60 
     money -=190

    if zakupy == "8":
     money-=500

    print(f"Masz {life} HP  {mana} many i {money} pięniędzy ")


print(f"Masz {life} HP  {mana} many i {money} pięniędzy ")


print( name +" wyjechałeś z wioski ale kiedy przejerzdrzałeś przez most zaatakował cię smok morski")
print("--1. (jeśli nie masz legendarnego miecza) Walczysz ze smokiem w sposób tradycyjny")
print("--2. (jeśli masz legendarny miecz) Ciskasz w smoka mieczem ")
print("--3. uciekasz ")

if zakupy =="8":
   print("Masz miecz")
if zakupy !="8":
   print("Nie masz miecza")

decyzja = input("podejmij decyzje")

if decyzja =="1":
   print("wygrywasz walke jednak tracisz 25 HP")
   life -= 25
   money += 300
   mana += 0

elif decyzja =="2":
   print("wygrywasz walke i nie tracisz HP ponieważ zabiłeś smoka za jednym ciosem")
   life += 0
   money +=350
   mana += 20

elif decyzja =="3":
   life -= 200
   money -=100
   mana -= 100
   if trudność =="3":
    print("Przegrałeś Koniec Gry!!!")
    quit()

if trudność !="3":
    print("żyjesz")
    life += 20


print(f"Masz {life} HP  {mana} many i {money} pięniędzy ")

print(name + " po walce ze smokiem dotarłeś do magicznego miejsca gdzie wymieniłeś skóre smoka na leczniczą miksture oraz dostałeś do wyboru 3 mittyczne przedmioty (możesz wybrać jeden) ")
print("--1. Zbroja z smoczych łósek")
print("--2. Topór wykuty w czeluściach góry irana")
print("--3. Kusze automatyczną króla kerena")

life += 80 
print(f"Masz {life} HP  {mana} many i {money} pięniędzy ")


oręż =input("wybież swój oręż")

if oręż =="1":
   print("posiadasz mityczną Zbroje") 
   
elif oręż =="2":
   print("posiadasz mityczny Topór ")

elif oręż =="3":
   print("posiadasz mityczną Kusze")

print("opuszczasz magiczną wioskke i chwile po rozpoczęciu podróży atakuje cie grupa mrocznych potworów (jest ich 3)")


print("--1. defensywa")
print("--2. ofensywa ")

walka = input("wybierz sposób walki")

if walka =="1":
   print("zostajesz zaatakowany przez 3 potwory na raz udaje ci się jednego zabic zadają ci 80 dmg")
   life -= 80
   mana -= 30
elif walka =="2":
   print("potwory nie spodziewają się ataku z twojesj strony zabijasz jednego i nie otrzymujesz obrażeń")
   life -= 0
   mana -= 10
print(f"Masz {life} HP  {mana} many i {money} pięniędzy ")

if oręż !="1":
   print("Nie masz Mitycznej Zbroji")
if oręż !="2":
   print("Nie masz Mitycznego Topora")
if oręż !="3":
   print("Nie masz Mitycznej Kuszy")
if oręż =="1":
   print("Masz Mityczną Zbroje")
if oręż =="2":
   print("Masz Mityczny Topór")
if oręż =="3":
   print("Masz Mityczną Kusze")
      
print("--1. wykorzystujesz mityczną Zbroje ")
print("--2. wykorzystujesz mityczny Topór")
print("--3 wykorzystujesz mityczną Kusze ")

walka2 = input("kontynuacja walki")

if walka2 =="1":
   print("otrzymujesz 100 hp a potwory zadały ci 50 zanim je zabiłeeś")
   life += 100
   life -= 50
   mana -= 15
   money += 70

elif walka2 =="2":
   print("atakujesz potwory wymachując toporem zabijasz je i otrzymujesz 100 Hp")
   life += 100
   mana -= 20
   money += 100

elif walka2 =="3":
   print("posyłasz w potwory salwe z kuszy zabijasz je bez otrzymania obrażeń")
   money += 100
   life += 0
   mana -= 10

print(f"Masz {life} HP  {mana} many i {money} pięniędzy ")

print("brawo pokonałeś podwładnych czarnoksiężnika lecz aby go pokonać musisz odnaleść zaklęcie (gdzie szukasz?)")

print('--1. przeszukujesz kosmiczny las')
print("--2. przeszukujesz magiczny dom")
poszukiwanie = input("")


if poszukiwanie =="2":
   print("brawo masz zaklęcie")
   
elif poszukiwanie =="1":
   print("--2. spróbuj jeszce raz tutaj nie znajdziesz tego czego szukasz")
   poszukiwanie = input("druga próba")
if poszukiwanie =="2":
   print("brawo masz zaklęcie")

print("Czeka cie ostateczna bitwa idziesz do zamku czarnoksiężnika gdzie on już czeka na ciebie z małą armią")
print("--1. urzywasz zaklęcia i pokonujesz armie carnoksiężnika")
print("--2. nie urzywasz zaklęcia i atakujesz bronią")

Ostatnia_walka = input("jak postąpisz?")

if Ostatnia_walka =="1":
   print("Zabiłeś potwory ale czrnoksięznik przerzył")
   life -= 0
   mana -= 50
   money += 300
elif Ostatnia_walka =="2":
   life -=1000
   mana -=100
   print("Umarłeś koniec gry")
   quit()

print("czarnoksiężnik wyzywa cie do pojedynku (ZAKOŃCZENIE)")
print("--1. atakujesz go z całą mocą")
zakończenie = input("wykończ czarnoksiężnika")

if zakończenie =="1":
   print("Gratulacje Zabiłeś czarnoksiężnika i uratowałeś świat ludzkość jest z ciebie dumna ")
   money += 1000
   mana -= 30
   life -= 25
   print(f"Masz {life} HP  {mana} many i {money} pięniędzy oto twój now rekord!!!!! ")
print("KONIEC GRY!!!!")
