# Machine-Learning-DesicionTree

## Desicion Tree
Bu, Iris veri kümesi üzerinde sınıflandırma için karar ağaçlarının kullanımını gösteren bir Python kodudur.

## Kütüphaneler İçe Aktarma ve Verilerin Yüklenmesi
İlk blokta, veri manipülasyonu için pandas, sayısal işlemler için numpy ve veri görselleştirme için matplotlib gibi gerekli kütüphaneler dahil edilir. Iris veri kümesi, pandas read_csv yöntemi kullanılarak içe aktarılır.

## Veri Setinin Eğitilmesi ve Test Setlerine Ayrılması
İkinci blok, veri kümesini modelleme için hazırlar. Bağımsız değişkenler X matrisinde depolanır ve bağımlı değişken (yani, iris türü) Y vektöründe depolanır. Veri kümesi, scikit-learn'den train_test_split işlevi kullanılarak eğitim ve test setlerine ayrılır ve verilerin %67'si eğitim, %33'ü test için kullanılır.

## Desicion Tree Algoritması Modelini Oluşturma
Üçüncü blokta, bir karar ağacı sınıflandırıcısı örneği oluşturulur ve eğitim verileri kullanılarak eğitilir. Eğitilmiş model, test verilerinde tahminler yapmak için kullanılır ve sonuçlar tahmin değişkeninde depolanır.

## Modelin Performansını Değerlendirme ve Doğruluğunu Hesaplama
Dördüncü blok, tahminlerin karışıklık matrisini hesaplar. Karışıklık matrisi, modelin doğru pozitiflerin (TP), yanlış pozitiflerin (FP), doğru negatiflerin (TN) ve yanlış negatiflerin (FN) sayısını gösteren bir tablodur. Sınıflandırma problemleri için bir performans ölçüsüdür. Bu durumda, karışıklık matrisi yazdırılır ve 50 test örneğinden 48'inin doğru sınıflandırıldığı görülür.
Son olarak, beşinci blok, scikit-learn'den accuracy_score işlevini kullanarak modelin doğruluğunu hesaplar. Doğruluk, toplam örnek sayısından doğru sınıflandırılan örneklerin oranıdır. Bu durumda, doğruluk 0,96 olarak yazdırılır, bu da modelin iyi performans gösterdiğini gösterir.
