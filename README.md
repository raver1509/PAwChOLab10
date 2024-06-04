# Sprawozdanie z Laboratorium 10

# Treść polecenia
Należy uruchomić trzy kontenery o nazwach odpowiednio: web1, web2, web3, które zawierać
będą serwery nginx w wersji latest w taki sposób by:
• wszystkie te serwery były podłączone do jednej sieci mostkowej definiowanej
przez użytkownika (nazwa sieci: lab10net),
• wszystkie serwery były dostępne z sieci zewnętrznej (z poziomu używanego
komputera, laptopa),
• poszczególne serwery wyświetlały prosta stronę html zawierającą: numer
laboratorium, imię i nazwisko studenta a strona ta została podłączona do każdego
z serwerów nginx wykorzystując wolumeny z uprawnieniami dostępu: read-only,
• poszczególne serwery zapisywały logi do trzech dedykowanych katalogów w
podkatalogu katalogu domowego o nazwie lab10. Katalog lab10 ma zostać
dołączony do kontenerów również wykorzystując wolumeny.
W sprawozdaniu proszę umieścić wszystkie użyte polecenia wraz z wynikiem ich działania.
Polecenia te powinny dowieść, że wszystkie trzy serwery poprawnie wyświetlają stronę
html a logi serwerów zostały poprawnie zapisane i są dostępne w systemie macierzystym
(z poziomu wykorzystywanego komputera, laptopa)

# Wykonanie polecenia

Utworzenie sieci bridge o nazwie lab10net
![image](https://github.com/raver1509/PAwChOLab10/assets/36925740/3c6f4791-caab-4270-9d00-d8e67b1a2a7a)

Utworzenie pliku html zawierającego stronę z informacją o imieniu i nazwisku studenta oraz numer laboratorium
![image](https://github.com/raver1509/PAwChOLab10/assets/36925740/e8fe101c-b466-4900-a5aa-70df6cca7bad)
![image](https://github.com/raver1509/PAwChOLab10/assets/36925740/0b8c39bd-ce9a-40d9-b6aa-dac55a914490)

Stworzenie katalogów na logi
![image](https://github.com/raver1509/PAwChOLab10/assets/36925740/4de1d5ec-951c-4f8a-9221-ee6c9420e459)

Uruchomienie kontenerów (dostęp do katalogu z plikiem zawierającym stronę w trybie read only)
![image](https://github.com/raver1509/PAwChOLab10/assets/36925740/f366e01a-f219-4394-9166-b95503ef1242)

Sprawdzenie istnienie utworzonych kontenerów w sieci lab10net
![image](https://github.com/raver1509/PAwChOLab10/assets/36925740/702d1d01-1c91-43f8-9d90-3498de39fc1f)

Sprawdzenie poprawnego zapisu logów oraz dostępu do nich z maszyny macierzystej
![image](https://github.com/raver1509/PAwChOLab10/assets/36925740/4e85edb7-e542-4a27-8bb6-a8aa0983a8b9)





