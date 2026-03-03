# OAI PREPARE 2025-26

Repozytorium zawiera materiały przygotowujące do **III Olimpiady Sztucznej Inteligencji (OAI)** edycji 2025/2026. Składa się z 16 modułów w formie notebooków Jupyter, prowadzących od podstaw Pythona aż do zaawansowanych technik fine-tuningu dużych modeli językowych.

---

## Spis modułów

### Moduł 0 – OAI Kompendium (`modul_00_oai_kompendium.ipynb`)
Przewodnik po wszystkich zadaniach z poprzednich edycji OAI (I–III). Zawiera:
- mapowanie 24+ zadań konkursowych na wymagane umiejętności,
- wzorzec `FINAL_EVALUATION_MODE` używany w każdym zadaniu,
- przegląd kluczowych metryk (accuracy, F1, PSNR, ROC AUC, BLEU, MRR@K, IoU),
- ranking 10 najczęściej testowanych umiejętności (PyTorch, metryki, CNN),
- dozwolone biblioteki oraz strategię nauki.

### Moduł 1 – Podstawy Pythona (`modul_01_python_podstawy.ipynb`)
Kompletne wprowadzenie do Pythona:
- typy danych, zmienne, konwersja typów, f-strings,
- operatory arytmetyczne, porównania, logiczne,
- listy, słowniki, zbiory, krotki,
- instrukcje sterujące: `if/elif/else`, `for`, `while`, `break/continue`,
- funkcje, funkcje lambda,
- klasy, dziedziczenie, OOP,
- list comprehensions i dict comprehensions,
- 10 ćwiczeń (FizzBuzz → Fibonacci → projektowanie klas).

### Moduł 2 – NumPy i losowość (`modul_02_numpy_losowosc.ipynb`)
Obliczenia naukowe – fundament ML:
- tworzenie tablic, indeksowanie, slicing,
- operacje element-wise, agregacje (sum, mean, std),
- algebra liniowa: iloczyn skalarny, mnożenie macierzy, normy,
- reshape, transpose, flatten,
- liczby losowe i ustawianie ziarna (reprodukowalność),
- broadcasting.
- 6 ćwiczeń: statystyki, ręczne mnożenie macierzy, normalizacja min-max, podobieństwo cosinusowe, Monte Carlo (π), softmax.

### Moduł 3 – Pandas i statystyka (`modul_03_pandas_statystyka.ipynb`)
Analiza danych tabelarycznych:
- tworzenie i manipulacja DataFrame/Series,
- wczytywanie i zapisywanie danych,
- eksploracja: `head`, `info`, `describe`, `dtypes`,
- filtrowanie, indeksowanie (`loc`/`iloc`),
- GroupBy i agregacje,
- obsługa brakujących wartości (NaN),
- statystyki opisowe: średnia, mediana, kwantyle, korelacja.
- 5 ćwiczeń: analiza ocen studentów, zaawansowane filtrowanie, tabele przestawne, kategoryzacja, symulacja danych pogodowych.

### Moduł 4 – Wizualizacja i EDA (`modul_04_wizualizacja_eda.ipynb`)
Eksploracyjna analiza danych (matplotlib & seaborn):
- podstawy matplotlib: figury, subploty, stylizacja,
- typy wykresów: scatter, histogram, boxplot, heatmap,
- zaawansowane wykresy seaborn: pairplot, rozkłady,
- macierze korelacji,
- 8-krokowy schemat EDA.
- 4 ćwiczenia: EDA na Iris, wizualizacja funkcji aktywacji, wykresy rozkładów, dashboard sprzedaży.

### Moduł 5 – Wstęp do ML (`modul_05_wstep_do_ml.ipynb`)
Kompleksowe podstawy uczenia maszynowego:
- uczenie nadzorowane, nienadzorowane, ze wzmocnieniem,
- podziały train/val/test i stratyfikacja,
- metryki: Accuracy, Precision, Recall, F1, Balanced Accuracy, ROC AUC,
- macierz konfuzji,
- overfitting vs underfitting,
- tradeoff bias-variance (z matematyką),
- regularyzacja: L1, L2, Elastic Net,
- walidacja krzyżowa (k-fold, LOO),
- preprocessing: standaryzacja, normalizacja, robust scaling,
- wyciek danych (data leakage),
- PCA i alternatywy (t-SNE, UMAP, LDA).
- 5 zadań + 3 dodatkowe zadania w stylu olimpijskim.

### Moduł 6 – Klasyczne algorytmy ML (`modul_06_klasyczne_ml.ipynb`)
Metody drzewowe i jądrowe:
- drzewa decyzyjne: nieczystość Giniego, zysk informacyjny, CART,
- regularyzacja drzew: max_depth, min_samples_split, przycinanie CCP,
- Random Forest: bootstrap aggregation, ważność cech,
- SVM: marginesy, sztuczka jądrowa, RBF,
- grid search do strojenia hiperparametrów.

### Moduł 7 – Regresja i gradient (`modul_07_regresja_gradient.ipynb`)
Fundamenty optymalizacji sieci neuronowych:
- regresja liniowa i równanie normalne,
- funkcja straty MSE i jej właściwości (wypukłość, gładkość),
- gradient descent: batch, stochastyczny, mini-batch,
- dobór współczynnika uczenia,
- momentum i inne optymalizatory,
- wprowadzenie do PyTorch.

### Moduł 8 – MLP w PyTorch (`modul_08_mlp_pytorch.ipynb`)
Sieci w pełni połączone:
- sztuczny neuron i perceptron,
- warstwy Dense: liczba parametrów,
- funkcje aktywacji: sigmoid, tanh, ReLU, Leaky ReLU, GELU, softmax,
- problem zanikającego gradientu i rozwiązania,
- projektowanie architektury MLP,
- forward pass i backpropagation,
- pętla treningowa w PyTorch (5 kroków),
- regularyzacja: L1/L2, dropout, early stopping, batch normalization.
- Ćwiczenia: MNIST, eksperymenty z architekturą, porównanie regularyzacji.

### Moduł 9 – CNN (`modul_09_cnn.ipynb`)
Sieci konwolucyjne do przetwarzania obrazów:
- operacja splotu 2D (cross-correlation), wielokanałowość (RGB),
- przewagi CNN nad MLP: rzadkie połączenia, współdzielenie wag, niezmienność na translację,
- hierarchia cech: krawędzie → tekstury → obiekty,
- filtry (detekcja krawędzi, rozmycie, wyostrzanie),
- parametry `Conv2d`: in_channels, out_channels, kernel_size, stride, padding,
- wzór na rozmiar wyjścia: $(W - K + 2P)/S + 1$,
- pooling: max pooling, average pooling,
- batch normalization,
- transfer learning (ResNet, VGG),
- przegląd detekcji obiektów i segmentacji.

### Moduł 10 – NLP i embeddingi (`modul_10_nlp_embeddingi.ipynb`)
Podstawy przetwarzania języka naturalnego:
- tokenizacja: word-level, char-level, BPE, WordPiece, SentencePiece,
- algorytm BPE (krok po kroku),
- tokeny specjalne: [CLS], [SEP], [PAD], [UNK],
- prawo Zipfa: rozkład częstości w tekście ($f \propto 1/r$),
- reprezentacje tekstu: Bag of Words, TF-IDF,
- embeddingi słów: Word2Vec (Skip-gram, CBOW), GloVe,
- podobieństwo cosinusowe do wyszukiwania semantycznego.

### Moduł 11 – RNN i LSTM (`modul_11_rnn_lstm.ipynb`)
Sieci rekurencyjne do danych sekwencyjnych:
- ograniczenia MLP dla danych sekwencyjnych,
- architektury RNN: many-to-one, one-to-many, many-to-many, seq2seq,
- równania Vanilla RNN: $h_t = \tanh(W_{xh}x_t + W_{hh}h_{t-1} + b_h)$,
- BPTT (Backpropagation Through Time),
- problem zanikającego/eksplodującego gradientu w RNN,
- LSTM: bramki (forget, input, output) i stan komórki,
- GRU (uproszczona alternatywa),
- bidirectionalne RNN,
- metryka Perplexity dla modeli językowych.

### Moduł 12 – Transformery (`modul_12_transformery.ipynb`)
Nowoczesna architektura głębokiego uczenia (BERT, GPT):
- motywacja: równoległość, zależności długodystansowe,
- mechanizm atencji: query, key, value,
- Scaled Dot-Product Attention: $\text{Attention}(Q,K,V) = \text{softmax}(\frac{QK^T}{\sqrt{d_k}})V$,
- stabilność numeryczna (odejmowanie max przed exp),
- Multi-Head Attention: wiele głowic równolegle,
- pozycyjne kodowanie (sinus/cosinus),
- enkoder vs dekoder transformera,
- Masked Attention (przyczynowe modelowanie języka),
- Vision Transformer (ViT): atencja na patchach obrazu,
- złożoność self-attention: $O(n^2 \cdot d)$.

### Moduł 13 – Fine-tuning LLM (`modul_13_llm_finetuning.ipynb`)
Praca z dużymi modelami językowymi:
- enkodery (BERT: MLM, bidirectional) vs dekodery (GPT: autoregresja, causal),
- tokenizacja BPE – szczegółowy opis,
- cele pre-treningu: MLM, next-token prediction,
- prawa skalowania (scaling laws),
- prompt engineering: few-shot, chain-of-thought, role-play,
- techniki fine-tuningu: pełny fine-tune, LoRA, adapter modules,
- RLHF (Reinforcement Learning from Human Feedback),
- katastrofalne zapominanie,
- instruction tuning.

### Moduł 14 – Bielik w praktyce (`modul_14_bielik_praktyka.ipynb`)
Praktyczny przewodnik po modelu Bielik-11B (używanym na olimpiadzie):
- specyfikacja: 11B parametrów, ~22 GB VRAM w bfloat16,
- kiedy używać Bielika: polski tekst, klasyfikacja, ekstrakcja,
- kiedy NIE używać: zadania czysto wizyjne, proste ML, obliczenia numeryczne,
- format ChatML: `<|im_start|>role\ncontent<|im_end|>`,
- ładowanie modelu przez `transformers` (AutoModelForCausalLM, AutoTokenizer),
- wzorce wnioskowania: few-shot, system prompts,
- optymalizacja promptów,
- zarządzanie pamięcią VRAM i techniki oszczędzania pamięci,
- obsługa limitów czasowych (2–5 min na wywołanie).

### Moduł 15 – Strategie zawodów (`modul_15_strategie_zawodow.ipynb`)
Taktyka na olimpiadę:
- format zawodów: ~5 h, notebooki Jupyter, GPU (T4 lub A100), brak internetu,
- dozwolone biblioteki: torch, torchvision, numpy, pandas, sklearn, matplotlib, nltk, transformers, xgboost, tqdm, Pillow,
- wzorzec `FINAL_EVALUATION_MODE`,
- strategia triaży: priorytetyzacja zadań wg trudności/nagrody,
- budżetowanie czasu na 4–6 problemów,
- debugowanie offline,
- checkpointy i reprodukowalność (ziarna losowości),
- pamięciowe wzory wszystkich kluczowych metryk,
- zarządzanie pamięcią GPU: bfloat16, kwantyzacja,
- typowe pułapki: data leakage, zła metryka, overfitting, limity czasu,
- lista kontrolna przed i w trakcie zawodów,
- 5+ gotowych szablonów kodu.

---

## Wymagania

Notebooki korzystają z następujących bibliotek (dostępnych na olimpiadzie):

```
torch torchvision numpy pandas scikit-learn matplotlib seaborn
nltk transformers xgboost tqdm Pillow
```

---

## Struktura nauki

```
Podstawy (0–5) → Klasyczne ML (6–7) → Głębokie uczenie (8–12) → LLM (13–15)
```

Moduł 0 pełni rolę przewodnika – warto do niego wracać przez cały czas przygotowań. Moduł 15 podsumowuje całość i zawiera strategie na sam dzień zawodów.
