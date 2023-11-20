Step-2-

İlk olarak web socket ve tcp socket bağlantısının gerçekleştiği nodejs uygulamasına göz atalım:

cat /root/socket/tcpsocket.js

Bu kod, WebSocket ve TCP'yi kullanarak iki farklı türde istemcilerle etkileşimde bulunur.

WebSocket İletişimi:

Bir WebSocket sunucusu oluşturulur ve 3000 portunda dinlemeye başlar.
Bir WebSocket istemcisi bu sunucuya bağlandığında, bağlantı kurulduğuna dair bir log mesajı yazdırılır.
WebSocket üzerinden gelen veriler dinlenir.
Gelen WebSocket verileri, aynı anda bir TCP sunucusuna yönlendirilir.

TCP İletişimi:

Ayrı bir TCP sunucusu oluşturulur ve 2000 portunda dinlemeye başlar.
Bir TCP istemcisi bağlandığında, bağlantı kurulduğuna dair bir log mesajı yazdırılır.
TCP sunucusundan gelen veriler dinlenir.
Gelen TCP verileri, bu sunucuya bağlı olan tüm WebSocket istemcilerine yönlendirilir.
Bu yapı, örneğin bir web tarayıcısından (WebSocket istemcisi) gelen verileri bir sunucuya alıp,
aynı zamanda bir başka sunucu (TCP sunucusu) ile iletişim kurarak alınan veriyi oraya yönlendirmek için kullanılabilir.
Bu, gerçek zamanlı uygulamalarda veya farklı ağ protokollerini birleştirmek istediğiniz diğer senaryolarda kullanışlı olabilir.
