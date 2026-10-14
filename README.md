# kulup-odevi
print('==Şifre Gücü Analizcisi==')
sifre=input('Şifreni gir: ')
if sifre=='8828':
    print('==EAL ROBOTİK<3==')
    exit()
while len(sifre)<8:
    print('Şifren çok kısa!(en az 8 karakter)')
    sifre=input('Tekrar dene: ')
while not any(karakter.insdigit()for karakter in sifre):
    print('Şifrede en az bir sayı olmalı!)
    sifre=input('Tekrar dene: ')
while not any(karakter.isupper()for karakter in sifre):
    print('Şifre büyük harf içermeli!')
    sifre=input('Tekrar dene: ')
while not any(not karakter.isalnum()for karakter in sifre):
    print('Özel karakter ekle!(boşluk,!,@,# gibi)')
    sifre=input('Tekrar dene:  ')
print('Şifren güvenilir!')