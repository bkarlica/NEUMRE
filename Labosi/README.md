# NEUMRE - Neuronske mreže

Laboratorijske vježbe iz neuronskih mreža, izrađene u Pythonu (Jupyter Notebook) uz biblioteke NumPy, SciPy, Matplotlib, PyTorch i scikit-learn.

## Lab 1: Model neurona i asocijativna memorija

**1. Model neurona i učenje.** 
**2. Asocijativna memorija.** 

Kod i komentari nalaze se u bilježnici [`lab1_KB.ipynb`](laboratory1/lab1_KB.ipynb).

## Lab 2: Perceptron i LMS algoritam

**3. Perceptron.** 

**4. LMS algoritam za predviđanje cijene dionice.**  Podaci se učitavaju iz datoteke [`stock.txt`](laboratory2/stock.txt).

Kod i komentari nalaze se u bilježnici [`lab2_KB.ipynb`](laboratory2/lab2_KB.ipynb).

## Lab 3: Višeslojni perceptron (PyTorch) i SVM

**5. Višeslojni perceptron u PyTorchu.** Nakon uvoda u PyTorch (tenzori, Dataset i DataLoader, modeli, optimizatori) riješila sam XOR problem malom mrežom s jednim skrivenim slojem i usporedila aktivacijske funkcije (sigmoid, tanh), optimizatore (SGD, Adam) i stope učenja prema broju epoha do konvergencije. Zatim sam trenirala potpuno povezanu mrežu za prepoznavanje rukom pisanih znamenki na skupu MNIST (točnost oko 97%) i usporedila utjecaj hiperparametara na točnost.

**6. Support Vector Machine (scikit-learn).** Usporedila sam linearni, RBF i polinomni kernel na skupu Iris (uz stratificiranu podjelu 70/30), istražila utjecaj odabira značajki na skupu Wine i izmjerila kako vrijeme treniranja SVM-a raste s veličinom skupa podataka (približno kvadratno).

Kod i komentari nalaze se u bilježnici `lab3_KB.ipynb`.

## Lab 4: Rekurentne i konvolucijske neuronske mreže

**7. LSTM na MNIST-u.** Slike znamenki obrađivala sam kao nizove redaka koje LSTM prima jedan po jedan. Ispitala sam kako točnost ovisi o broju redaka koje mreža vidi (mreža ne mora vidjeti cijelu sliku za točnu klasifikaciju) te usporedila optimizatore Adam i SGD s momentumom.

**8. Konvolucijske neuronske mreže (PyTorch).** Na MNIST-u sam izgradila CNN (točnost oko 99%), usporedila arhitekture po broju parametara i točnosti te isprobala aktivacijske funkcije LeakyReLU i ELU. Zatim sam koristila prednaučene mreže (ResNet34, VGG16) za klasifikaciju slika i kao ekstraktore značajki za SVM klasifikatore: škare naspram kliješta te zdrava naspram nezdrave hrane. VGG16 se pokazao boljim ekstraktorom značajki od ResNet34 u oba zadatka.

Kod i komentari nalaze se u bilježnici `lab4_KB.ipynb`. Slike za zadatke klasifikacije nalaze se u mapi `cnn_img`.
