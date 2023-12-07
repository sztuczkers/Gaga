from random import randint
print("podaj imie bohatera")
name = input()
print ("witaj " + name) 

life = 100 
mana = 300 
money = 500

print(f"Masz {life} HP  {mana} many i {money} pięniędzy ")

print("Aby zagrać wybierz poziom trudności")

print ("1. bardzolatwy")
print ("2. latwy")
print ("3. sredni")
print("4. trudny")
print ("5. bardzotrudny")

trudność = input("Wybierz poziom trudności ")

if trudność == '1':
    print("wybrałeś poziom bardzolatwy kliknj 1 aby rozpocząć rozgrywke")
    życia = 5
elif trudność == "2":
    print("wybrałeś poziom latwy kliknj 2 aby rozpocząć rozgrywke")
    życia = 4
elif trudność == "3":
    życia = 3
    print("wybrałeś poziom sredni kliknj 3 aby rozpocząć rozgrywke")
elif trudność == "4":
    życia = 2
    print("wybrałeś poziom trudny kliknj 4 aby rozpocząć rozgrywke")
elif trudność == "5":
    życia = 1
    print("wybrałeś poziom bardzotrudny kliknj 5 aby rozpocząć rozgrywke")
gra = input("Omówienie ")

if gra == "1":
    print("Witaj aby wygrać musisz dokonywać własciwych wyborów jeśli wybierzesz źle tracisz życie na poziomie bardzolatwtym masz 5 życia będziesz miał do wyboru od 2 do 4 opcji jeśli wybierzesz tracisz hp ")
if gra == "2":
    print("Witaj aby wygrać musisz dokonywać własciwych wyborów jeśli wybierzesz źle tracisz życie na poziomie latwym masz 4 życia będziesz miał do wyboru od 2 do 4 opcji jeśli wybierzesz tracisz hp ")
if gra == "3":
    print("Witaj aby wygrać musisz dokonywać własciwych wyborów jeśli wybierzesz źle tracisz życie na poziomie sredni masz 3 życia będziesz miał do wyboru od 2 do 4 opcji jeśli wybierzesz tracisz hp  ")
if gra == "4":
    print("Witaj aby wygrać musisz dokonywać własciwych wyborów jeśli wybierzesz źle tracisz życie na poziomie trudnym masz 2 życia będziesz miał do wyboru od 2 do 4 opcji jeśli wybierzesz tracisz hp  ")
if gra == "5":
    print("Witaj aby wygrać musisz dokonywać własciwych wyborów jeśli wybierzesz źle tracisz życie na poziomie bardzotrudnym masz 1 życia będziesz miał do wyboru od 2 do 4 opcji jeśli wybierzesz tracisz hp  ")


print (" kliknij 1 aby zapoznać się z fabułą gry")

start = input("Wprowadzenie faburalne")

if start == "1":
    print("W magicznym królestwie, bohater wyrusza na wyprawę, by pokonać mroczne potwory zwiastujące nadejście chaosu. Musi odkryć zaklęcia i odnaleźć legendarną broń, by uratować świat przed zgubą.")



print(name  + "jesteś podczas kolejnej wyprawy, atakuje cie  lis oto twoje opcje ")
print("1- walczysz z lisem")
print("2- omijasz go jadąc przez las")

decyzja = input("podejmij decyzje ")

if decyzja == "1":
    print("wygrałeś i sprzedałeś skóre lisa  masz teraz ")
    life -= 10
    mana -= 20
    money += 100


elif  decyzja =="2":
    print("w lesie znajdujesz monety ale kaleczysz się o krzak więc tracisz hp")
    life -= 20
    money += 100

print(f"Masz {life} HP  {mana} many i {money} pięniędzy ")

print( name  + " przejerzdżasz obok wioski (muszisz jechać do sklepu)")
print("1- jedziesz do sklepu")
decyzja = input("zdecyduj się")
if decyzja == "1":
    print("możesz kupić następujące towary")
    
    print("1. mikstura_zdrowia")
    print("2. mikstura_siły")
    print("3. tarcza")
    print("4. zbroja")
    print("5. mityczna broń ktora mozesz  pokonać  potwory")
    print("możesz  kupić tylko 1 rzecz")

    zakupy = input("wybierz co chesz kupić")
      
if zakupy == "1":
      life+=30
      money-=50
if zakupy == "2":
     mana+=20 
     money-=60

if zakupy == "3":
     life+= 30 
     money-=120

if zakupy == "4":
     life+= 20 
     money -=150

if zakupy == "5":
     money-=300

print(f"Masz {life} HP  {mana} many i {money} pięniędzy ")


print(f"Masz {life} HP  {mana} many i {money} pięniędzy ")


print( name +" wyjechałeś z wioski ale kiedy przejerzdrzałeś przez most zaatakował cię smok ")
print("1. (jeśli nie masz mitycznego miecza) walczysz ze smokiem w sposób tradycyjny")
print("2. (jeśli masz legendarny miecz) walczysz ze smokiem mitycznym mieczem  ")
print("3. uciekasz ")

if zakupy =="8":
   print("Masz miecz")
if zakupy !="8":
   print("Nie masz miecza")

decyzja = input("podejmij decyzje")

if decyzja =="1":
   print("wygrywasz walke ale tracisz 50 HP")
   life -= 50
   money += 300
   mana += 20

elif decyzja =="2":
   print("wygrywasz walke i nie tracisz HP ponieważ zabiłeś smoka za jednym ciosem")
   life += 0
   money +=300
   mana += 20

elif decyzja =="3":
   life -= 200
   money -=200
   mana -= 50
   if trudność =="3":
    print("Przegrałeś Koniec Gry!!!")
    quit()

if trudność !="3":
    print("żyjesz")
    life += 20


print(f"Masz {life} HP  {mana} many i {money} pięniędzy ")

print(name + " po walce ze smokiem dotarłeś do magicznego miejsca gdzie wymieniłeś skóre smoka na leczniczą miksture oraz dostałeś do wyboru 3 mityczne przedmioty (możesz wybrać jeden) ")
print("1. Zbroja z smoczych łósek")
print("2. Topór wykuty w czeluściach góry irana")
print("3. Kusze automatyczną króla kerena")

life += 80 
print(f"Masz {life} HP  {mana} many i {money} pięniędzy ")


oręż =input("wybież swój oręż")

if oręż =="1":
   print("posiadasz mityczną Zbroje") 
   
elif oręż =="2":
   print("posiadasz mityczny Topór ")

elif oręż =="3":
   print("posiadasz mityczną Kusze")

print("opuszczasz  wioske i chwile po rozpoczęciu podróży atakuje cie grupa bandytow(jest ich 3)")


print("1. defensywa")
print("2. ofensywa ")

walka = input("wybierz sposób walki")

if walka =="1":
   print("zostajesz zaatakowany przez 3 bandytow na raz udaje ci się jednego zabic zadają ci 50 hp")
   life -= 50
   mana -= 30
elif walka =="2":
   print("bandyci nie spodziewają się ataku z twojej strony zabijasz jednego i nie otrzymujesz obrażeń")
   life -= 0
   mana -= 15
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
   print("otrzymujesz 120 hp a bandyci zadali ci 80 zanim je zabiłeeś")
   life += 120
   life -= 80
   mana -= 20
   money += 70

elif walka2 =="2":
   print("atakujesz bandytow  toporem zabijasz je i otrzymujesz 100 Hp")
   life += 100
   mana -= 15
   money += 110

elif walka2 =="3":
   print("posyłasz w bandytow salwe z kuszy zabijasz je bez otrzymania obrażeń")
   money += 150
   life += 0
   mana -= 20

print(f"Masz {life} HP  {mana} many i {money} pięniędzy ")

print("brawo pokonałeś podwładnych czarnoksiężnika lecz aby go pokonać musisz odnaleść zaklęcie (gdzie szukasz?)")

print('1. przeszukujesz kosmiczny las')
print("2. przeszukujesz magiczny dom")
poszukiwanie = input("")


if poszukiwanie =="2":
   print("brawo masz zaklęcie")
   
elif poszukiwanie =="1":
   print("2. spróbuj jeszce raz tutaj nie znajdziesz tego czego szukasz")
   poszukiwanie = input("druga próba")
if poszukiwanie =="2":
   print("brawo masz zaklęcie")

print("Czeka cie ostateczna bitwa idziesz do zamku czarnoksiężnika ")
print("1. urzywasz zaklęcia i go pokonujesz")
print("2. nie urzywasz zaklęcia i atakujesz bronią")

Ostatnia_walka = input("jak postąpisz?")

if Ostatnia_walka =="1":
   print("Zabiłeś  czarnoksięznika")
   life -= 0
   mana -= 50
   money += 300

elif Ostatnia_walka =="2":
   life -=1000
   mana -=100
   print("Umarłeś koniec gry")
   quit()

zakończenie = input("zabiles czarnoksięznika")
if zakończenie =="1":
   
   print("Gratulacje Zabiłeś czarnoksiężnika ")
   money += 1000
   mana -= 30
   life -= 25
   print(f"Masz {life} HP  {mana} many i {money} pięniędzy oto twój nowy rekord!!!!! ")
print("KONIEC GRY!!!!")
