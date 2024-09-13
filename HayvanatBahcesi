class Animal:
    def __init__(self,tur):
        self.tur=tur
    def bilgi(self):
        print(f"Tur:{self.tur}")
class Mammal(Animal):
    def __init__(self,tur,agirlik,hiz):
        super().__init__(tur)
        self.agirlik=agirlik
        self.hiz=hiz
    def bilgi(self):
        super().bilgi()
        print(f"Ağırlık:{self.agirlik}, Hız:{self.hiz}")
class Bird(Animal):
    def __init__(self,tur,kanatAcikligi):
        super().__init__(tur)
        self.kanatAcikligi=kanatAcikligi
    def bilgi(self):
        super().bilgi()
        print(f"Kanat açıklığı: {self.kanatAcikligi}")
class Reptile(Animal):
    def __init__(self,tur,uzunluk):
        super().__init__(tur)
        self.uzunluk=uzunluk
    def bilgi(self):
        super().bilgi()
        print(f"Uzunluk: {self.uzunluk}")
class Bakici:
    def __init__(self,isim,calisanID):
        self.isim=isim
        self.calisanID=calisanID
        self.hayvanlar=[]
    def hayvanAtama(self,hayvan):
        self.hayvanlar.append(hayvan)
        print(f"{self.isim}isimli bakıcıya {hayvan.tur} hayvanı atandı")
    def hayvanlariGoster(self):
        print(f"{self.isim}isimli bakıcının hayvanları:")
        for hayvan in self.hayvanlar:
            hayvan.bilgi()


class HayvanatBahcesi:
    def __init__(self):
        self.bakicilar=[]
    def bakiciEkle(self,bakici):
        self.bakicilar.append(bakici)
    def bakicilariGoster(self):
        for bakici in self.bakicilar:
            bakici.hayvanlariGoster()

fil=Mammal("Fil",5000,31)
aslan=Mammal("Aslan",192,78)
kartal=Bird("Kartal",2.5)
yilan=Reptile("Yılan",4)
bakici1=Bakici("Ahmet",200)
bakici2=Bakici("Elif",201)
bakici1.hayvanAtama(fil)
bakici2.hayvanAtama(aslan)
bakici1.hayvanAtama(kartal)
bakici2.hayvanAtama(yilan)
hayvanatBahce=HayvanatBahcesi()
hayvanatBahce.bakiciEkle(bakici1)
hayvanatBahce.bakiciEkle(bakici2)
hayvanatBahce.bakicilariGoster()
        
