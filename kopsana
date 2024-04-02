class Produkts:
    def __init__(self, nosaukums, cena, daudzums):
        self.nosaukums = nosaukums
        self.cena = cena
        self.daudzums = daudzums

class IepirkumuSaraksts:
    def __init__(self):
        self.produkti = []

    def pievienot_produktu(self, produkts):
        self.produkti.append(produkts)

    def parādīt_sarakstu(self):
        if not self.produkti:
            print("Saraksts ir tukšs.")
        else:
            print("Produktu saraksts:")
            for idx, produkts in enumerate(self.produkti, 1):
                print(f"{idx}. {produkts.nosaukums} - Cena: {produkts.cena} - Daudzums: {produkts.daudzums}")

def galvenais():
    iepirkumu_saraksts = IepirkumuSaraksts()

    while True:
        print("\nIzvēlieties darbību:")
        print("1. Pievienot produktu")
        print("2. Parādīt produktu sarakstu")
        print("3. Iziet")

        izvēle = input("Ievadiet darbības numuru: ")

        if izvēle == '1':
            nosaukums = input("Ievadiet produkta nosaukumu: ")
            cena = float(input("Ievadiet produkta cenu: "))
            daudzums = int(input("Ievadiet produkta daudzumu: "))
            produkts = Produkts(nosaukums, cena, daudzums)
            iepirkumu_saraksts.pievienot_produktu(produkts)
            print(f"{produkts.nosaukums} pievienots sarakstam.")
        elif izvēle == '2':
            iepirkumu_saraksts.parādīt_sarakstu()
        elif izvēle == '3':
            print("Izeja no lietotnes.")
            break
        else:
            print("Nepareiza ievade. Lūdzu, izvēlieties pareizu darbību.")

if __name__ == "__main__":
    galvenais()
