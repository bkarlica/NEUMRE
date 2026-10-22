# Prepoznavanje tumora iz MRI slika mozga

Timski projekt s FER-a (Python, PyTorch, TensorFlow, OpenCV). Cilj je bio klasificirati MRI snimke mozga u četiri klase (gliom, meningeom, tumor hipofize, bez tumora) pomoću konvolucijskih neuronskih mreža te usporediti različite arhitekture.

Korišten je javni Brain Tumor MRI Dataset s Kagglea (7023 slike). Usporedili smo tri modela: CNN s dilatiranim konvolucijama i pojednostavljeni EfficientNet (oba trenirana od nule) te prednaučeni EfficientNet-B3. Dodatno smo ispitali utječe li na rezultat prethodno izdvajanje regije mozga (ROI) iz slike.

Najbolji rezultat postigao je EfficientNet-B3 uz ROI ekstrakciju, s točnošću od oko 99,4%.

Cijeli izvještaj nalazi se u datoteci `MRI_projekt.pdf`, a prezentacija u `MRI_ppt.pptx`.

**Autori:** Lucija Topolko, Julijana Kolarec, Karla Budimir, Carla Goluža, Dora Bilić Pavlinović
