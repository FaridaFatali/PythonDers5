# PythonDers5
Python Kamp. Ders 5. Odev 1.

PyTestDecorators
Decorators in PyTest Bir Python dekoratörü, bir işlevi alıp, bazı işlevler ekleyip onu döndüren bir fonksiyondur. Python, fonksiyon çağrısını bir değişkene atamak yerine, @ sembolünü kullanarak bu işlevselliği elde etmek için çok daha zarif bir yol sağlar. Test zamanı bu gibi decorator’ler kullanabiliriz. Mesela:

@pytest.mark.skipif()
Parametresine boolean ve reason yazmak lazım, yani bu sepepten dolayı burada olanın geçerli olup olmadığını kontrol et, eğer bunlar geçerliyse o zaman skip et, yani bu fonksiyonu geç, test etme, ertele. Ve buraya da parametreleri str olarak yazıyoruz.

@pytest.mark.skip()
Parametre olmadan yazabiliriz, ama bir sepet de (reason) yazabiliriz, bu zaman o sepet str olarak yazılır. Bu decorator’ün yazıldığı fonksiyon test’den geçmiyor, onu erteliyor.

@pytest.fixture()
Bir fikstür fabrika fonksiyonunu işaretlemek için dekoratör. Bu dekoratör, bir fikstür fonksiyonunu tanımlamak için parametreli veya parametresiz olarak kullanılabilir.

@pytest.mark.filterwarnings()
Belirli test öğelerine uyarı filtreleri eklemek için kullanabilirsiniz, böylece test, sınıf ve hatta modül düzeyinde hangi uyarıların yakalanması gerektiğini daha iyi kontrol edebilirsiniz.

@pytest.mark.parametrize()
Bu dekoratör, bir test fonksiyonu için argümanların parametrizasyonunu sağlar. Burada, belirli bir girdinin beklenen bir çıktıya yol açıp açmadığını kontrol eden tipik bir test fonksiyonu örneği verilmiştir. Parametre olarak gerekli olanları str olarak ve liste olarak yazıyoruz.
