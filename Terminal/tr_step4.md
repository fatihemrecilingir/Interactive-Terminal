Step-4-

Web arayüzü için xterm uygulamasının htmll ve css dosyaları kullanılmıştır.

cat /root/xterm-terminal-demo/index.html

Bu HTML ve JavaScript kodu, bir web sayfasında etkileşimli bir terminal oluşturur. Kullanıcı, bu terminal aracılığıyla 
bir WebSocket bağlantısı üzerinden sunucuya komut gönderebilir ve sunucudan gelen cevapları görebilir.
Kullanıcı, gerçek bir terminal deneyimi yaşar ve sunucu ile etkileşimde bulunabilir.

Yine bu dizindeki server.js dosyası ile nodejs express modülünü kullanarak, 9999 portunda index.html'i yayınlayabiliriz.
