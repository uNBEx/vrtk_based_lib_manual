# Instrukcja do biblioteki

- [Instrukcja do biblioteki](#instrukcja-do-biblioteki)
  - [1. Tworzenie projektu](#1-tworzenie-projektu)
  - [2. Podstawowe funkcje VR](#2-podstawowe-funkcje-vr)
  - [3. Podłoże do poruszania się](#3-podłoże-do-poruszania-się)

## 1. Tworzenie projektu
1. Tworzymy nowy projekt Unity z szablonu `3D`.
2. Dodajemy `XR Plugin Management`:

        Edit -> Project Settings -> XR Plugin Management -> Install XR Plugin Management
3. Zaznaczamy `Oculus`
4. Logujemy się / tworzymy konto w Unity Asset Store https://assetstore.unity.com/
5. Dodajemy do swojego konta [VRTK v4 Tilia Package Importer](https://assetstore.unity.com/packages/tools/utilities/vrtk-v4-tilia-package-importer-214936)
6. Następnie instalujemy dodany asset:
   
        Window -> Package Manager
7. W górnym menu `Packages` wybieramy `My Assets`
8. Pobieramy i importujemy `VRTK v4 Tilia Package Importer`
9. Dodajemy Scoped Registry do `mainfest.json` projektu:

        Window -> Tilia -> Package Importer -> Add Scoped Registry
10. Instalujemy wszystkie dostępne paczki poza `oculusintegration` i `steamvr`

## 2. Podstawowe funkcje VR

1. Usuwamy domyślną kamerę `Main Camera`
2. Dodajemy unitypackage z assetami:
   
        Assets -> Import package -> Custom package
3. Z zaimportowanego folderu `MyPrefabs` przeciągamy prefab `Base` do hierarchii

## 3. Podłoże do poruszania się

1. Dodajemy kostkę:

        PPM w hierarchii -> 3D Object -> Cube
2. Ustawiamy pozycję na `X: 0, Y: -0.5, Z: 0`
3. Ustawiamy skalę w osiach X i Z na `10`
4. Nadajemy kostce tag `Teleportable`
5. Testujemy działanie

