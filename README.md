# django

# 1> Django projekt létrehozása

pip install django

### csekkoljuk a telepítés, hozzunklétre egy main.py-t

code'''
import django
print(django.get_version())
'''code 

# 2> Django projekt inicializálás

### a Python projekt az a Pythonhoz tartozó mindenféle modul kezelésére is szolgál egyébként, a Djangonak pedig van egy saját fogalma és ezt a django-admin nevű command line parancssoros vezérlővel lehet létrehozni.

### django-admin

### a projekt fogalom a django-ban gyakorlatilag az a gyűjtő, amivel mi majd az alkalmazásunkat létrehozzuk. Ez pedig úgy néz ki:

### django-admin startproject mysite .

### projekt neve : mysite
### . -al jelöljük hogy az aktuális mappába hozzon létre egy projektet és ne hozzon létre neki egy új mappát

### most létrehozott nekünk egy manage.py fájlt, ami a django projekthez tartozó management command line eszköz készlet lesz.

### a manage.py a django-hoz tartozó cli eszköz készlete, amivel majd minden dolgot tudunk létrehozni és futtani.

### a mysite mappában pedig a projekthez tartozó konfigurációs dájlok lesznek.

### a settings.py-ban vannak ténylegesen a beállítások, amit a projekt használói tudnak majd használni

### urls.py itt vannak azok az elérési utak, amiket kiakarunk szólgálni, mondjuk amikor valaki böngészőben megnézi az oldalt.

### az asgi.py és wsgi.py fájlok ezek majd akkor lesznek relevánsak, ha majd ezt az alaklmazást ki akarjuk telepíteni publikusan, akkor el kell dönteni milyen futtató környezetben vannak a projektünk futtatva, most ez jelenleg nekünk nem szükséges foglalkozni vele.

 