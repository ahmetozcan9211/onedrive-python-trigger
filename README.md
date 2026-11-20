# OneDrive → Python Otomasyon Tetikleyici

OneDrive'a bir dosya yüklendiğinde Python uygulamasını otomatik tetikleyip dosyayı işlemenin üç farklı mimarisini karşılaştıran ve örnekleyen proje.

> Bu depo bir proje vitrinidir. Kaynak kod paylaşılmamaktadır.

## Yöntemler

| # | Mimari | Ne zaman tercih edilir |
|---|---|---|
| 1 | **Power Automate Cloud + Desktop:** Bulut tetikleyici dosyayı PAD'e iletir, PAD Python'u çalıştırır | Microsoft ekosistemi standart olduğunda |
| 2 | **Power Automate → HTTP webhook:** Bulut akışı dosyayı Python web servisine POST eder | Sunucuda sürekli çalışan bir servis varsa |
| 3 | **Yerel klasör izleyici:** Senkronize OneDrive klasörü dosya sistemi olaylarıyla izlenir | Lisans veya bulut erişimi kısıtlıysa |

Her yöntem için adım adım kurulum rehberi ve çalışan örnek kod hazırlandı.

## Teknolojiler

`Python` · `watchdog` · `pandas` · `Power Automate` · `OneDrive`
