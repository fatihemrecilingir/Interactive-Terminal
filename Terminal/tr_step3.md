Step-3-

Bu imagede olmasa da server tarafında bir server.js dosyası var. İleriki sürümlerde hem client hem de server aynı image'i kullanabilecek.

Bu JavaScript kodu, bir TCP sunucusu oluşturarak belirli bir portu dinler. Gelen verileri işleyip,
"char" methodunu taşıyan verileri diğer IP adreslerine yönlendirir, "Command" methodunu taşıyan istekler ise
komut satırında çalıştırılır ve istekleri tüm clientlara döner.
Bu yönlendirme işlemi, client.txt dosyasındaki diğer IP adreslerine gönderim yaparak gerçekleştirilir.
