# Laboratorijske vježbe

Laboratorijske vježbe iz neuronskih mreža, izrađene u Pythonu (Jupyter Notebook) uz biblioteke NumPy, SciPy, Matplotlib, PyTorch i scikit-learn.

## Lab 1: Model neurona i asocijativna memorija

**1. Model neurona i učenje.** Implementirala sam model neurona s tri ulaza i pragom te tri aktivacijske funkcije (step, rampa, sigmoida). Od toga sam složila mrežu od tri neurona, a na jednom neuronu sam delta pravilom naučila logičku funkciju AND i pratila pogrešku kroz iteracije za različite stope učenja.

**2. Asocijativna memorija.** Izradila sam korelacijsku matricu koja pamti parove ključ-riječ (riječi su kodirane ASCII vrijednostima). Istražila sam što se događa s ortogonalnim, linearno ovisnim i neortogonalnim ključevima, kapacitet memorije te ortonormalizaciju ključeva (Gram-Schmidt) i izračun matrice pomoću inverza.

Kod i komentari nalaze se u bilježnici `lab1_KB.ipynb`.

## Lab 2: Perceptron i LMS algoritam

**3. Perceptron.** Implementirala sam perceptron i njegovo učenje LMS pravilom te ga primijenila na klasifikaciju točaka u 2D i 3D prostoru. Isprobala sam linearno odvojive skupove, XOR problem (koji perceptron ne može riješiti jer nije linearno odvojiv), klase s Gaussovom razdiobom i mrežu od dva perceptrona za klasifikaciju u četiri klase (binarno kodirani izlazi). Granice odluke i pogreška kroz epohe prikazani su grafovima.

**4. LMS algoritam za predviđanje cijene dionice.** Linearni neuron treniran LMS algoritmom koristi cijene iz nekoliko prethodnih dana za predviđanje današnje cijene dionice. Podaci se učitavaju iz datoteke `stock.txt`.

Kod i komentari nalaze se u bilježnici `lab2_KB.ipynb`.

## Lab 3: Višeslojni perceptron (PyTorch) i SVM

**5. Višeslojni perceptron u PyTorchu.** Nakon uvoda u PyTorch (tenzori, Dataset i DataLoader, modeli, optimizatori) riješila sam XOR problem malom mrežom s jednim skrivenim slojem i usporedila aktivacijske funkcije (sigmoid, tanh), optimizatore (SGD, Adam) i stope učenja prema broju epoha do konvergencije. Zatim sam trenirala potpuno povezanu mrežu za prepoznavanje rukom pisanih znamenki na skupu MNIST (točnost oko 97%) i usporedila utjecaj hiperparametara na točnost.

**6. Support Vector Machine (scikit-learn).** Usporedila sam linearni, RBF i polinomni kernel na skupu Iris (uz stratificiranu podjelu 70/30), istražila utjecaj odabira značajki na skupu Wine i izmjerila kako vrijeme treniranja SVM-a raste s veličinom skupa podataka (približno kvadratno).

Kod i komentari nalaze se u bilježnici `lab3_KB.ipynb`.

## Lab 4: Rekurentne i konvolucijske neuronske mreže

**7. LSTM na MNIST-u.** Slike znamenki obrađivala sam kao nizove redaka koje LSTM prima jedan po jedan. Ispitala sam kako točnost ovisi o broju redaka koje mreža vidi (mreža ne mora vidjeti cijelu sliku za točnu klasifikaciju) te usporedila optimizatore Adam i SGD s momentumom.

**8. Konvolucijske neuronske mreže (PyTorch).** Na MNIST-u sam izgradila CNN (točnost oko 99%), usporedila arhitekture po broju parametara i točnosti te isprobala aktivacijske funkcije LeakyReLU i ELU. Zatim sam koristila prednaučene mreže (ResNet34, VGG16) za klasifikaciju slika i kao ekstraktore značajki za SVM klasifikatore: škare naspram kliješta te zdrava naspram nezdrave hrane. VGG16 se pokazao boljim ekstraktorom značajki od ResNet34 u oba zadatka.

Kod i komentari nalaze se u bilježnici `lab4_KB.ipynb`. Slike za zadatke klasifikacije nalaze se u mapi `cnn_img`.
