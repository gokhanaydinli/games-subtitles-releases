# Altyazı — indirme

PS5 oyunlarındaki İngilizce altyazıyı okuyup TV'de oyunun üstünde Türkçe gösteren programın kurulum dosyaları.

**Kurulum ve kullanım:** https://gokh4n.dev/altyazi

Bu depoda kod yoktur; yalnız sürümler (Releases) durur:

- `Altyazi-Kurulum.exe`: Windows programı (Windows 10/11, yönetici izni istemez).
- `Altyazi-mac.zip`: macOS programı (deneysel).
- `altyazi-tv.apk`: Android TV uygulaması. Programın panelindeki adresten de iner.
- `altyazi-lg.ipk`: LG webOS TV uygulaması (deneysel).
- `altyazi-samsung.wgt`: Samsung Tizen TV uygulaması (deneysel).
- `surum.json` ve `surum.json.imza`: Programın kendini güncellerken okuduğu, imzalı sürüm bilgisi.

Program yalnız imzası doğru olan güncellemeyi kurar; indirilen dosyanın parmak izi `surum.json` içindekiyle
karşılaştırılır.

Bu program Sony Interactive Entertainment ya da oyun yayıncılarıyla bağlantılı değildir.

Sürümler, ana sunucudaki imzalı sürüm bilgisinden otomatik alınır (`.github/workflows/yansit.yml`): imza bu depodaki
açık anahtarla (`guncelleme-acik.pem`) doğrulanır, dosyaların parmak izi karşılaştırılır; tutmazsa yayınlanmaz.
