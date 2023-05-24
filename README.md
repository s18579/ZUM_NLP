# Projekt NLP ZUM
<a href="https://colab.research.google.com/drive/1Vs4Diav8Nqztfm7moZ6L8wPpStyI1UrR?usp=sharing" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

## Spis tresci
- [Opis Projektu](#opis-projektu)
- [Setup](#setup)
- [Etap 1: Zbieranie Danych](#etap-1-zbieranie-danych)
- [Etap 2: Classic ML](#etap-2-classic-ml)
- [Etap 3: Neural Model](#etap-3-neural-model)
- [Etap 4: Language Model](#etap-4-language-model)

## Opis Projektu
Realizowany Projekt Natural Language Processing (NLP) jako końcowy projekt z przedmiotu ZUM ma na celu stworzenie modelu analizy sentymentu opartego na tweetach dotyczących aktualnych wydarzeń na świecie, w tym przypadku analiza sentymentu o królu Karolu III między śmiercią królowej Elżbiety II a jego koronacją. Projekt został stworzony jako notatnik Jupyter `.ipynb` w środowisku Google Colab.

## Setup
Cały projekt został zorganizowany tak, aby każdy etap mógł być uruchamiany osobno w środowisku Google Colab. Dla każdego etapu wymagane są odpowiednie biblioteki, które są instalowane na początku każdego z etapów. To czyni projekt elastycznym i łatwym do replikacji w różnych środowiskach.

W przypadku używania danego notatnika na lokalnym IDE rekomendowane jest zainstalowanie danych bibliotek zawartych w każdej z sekcji w podsekcji `Instalacja bibliotek`.

## Etap 1: Zbieranie Danych
W tym etapie, za pomocą narzędzia `snscrape`, zgromadzono 22,5 tys. tweetów dotyczących króla Wielkiej Brytanii Karola III, zbierając dane z zakresu od 1 września 2022 (od śmierci królowej Elżbiety II) do 31 maja 2023 (koronacji Karola III). Proces ten obejmował instalację niezbędnych bibliotek, import bibliotek, zbieranie danych z Twittera, a następnie zapis tych danych do pliku CSV. Następnie, dane były czyszczone i przygotowywane do dalszej analizy. Zostało to zrealizowane za pomocą własnostworzonych funkcji do czyszczenia danych.

## Etap 2: Classic ML
Drugi etap koncentrował się na zastosowaniu klasycznych technik uczenia maszynowego do przewidywania sentymentu. Użyto tutaj kilka algorytmów, w tym Naiwny Bayes, Regresja Logistyczna i Drzewa Decyzyjne. Każdy z tych modeli został odpowiednio przeszkolony i zwizualizowany, aby zrozumieć jego skuteczność i wyniki.

## Etap 3: Neural Model
Na tym etapie projektu zastosowano model BLSTM. Po instalacji i imporcie potrzebnych bibliotek, dane były przygotowywane do przetwarzania przez sieć neuronową. Następnie model został przeszkolony jak i również dostrajany, aby uzyskać najlepszy wynik (w tym przypadku prawie 90% accuracy na bazie danych testowych), zwizualizowany i przetestowany.

## Etap 4: Language Model
Czwarty etap skupiał się na zastosowaniu modelu języka, konkretnie DistilBERT, jednego z modeli Transformer BERT. Przygotowanie danych do tego modelu było podobne do etapu 3, ale uwzględniało specyfikę modelu BERT. Model został następnie przeszkolony i przetestowany, aby ocenić jego skuteczność w analizie sentymentu tweetów.

