Yapmış olduğum Valf fonksiyon bloğu hidrolik ve pnömatik sistemler için uygundur.
![Uploading 2024-08-21_13h59_21.png…]()


Input
Mod_Man : Sitemin Manuel Moda Alında True Yapılır
Mod_Auto: Sitemin Otomatik Moda Alında True Yapılır
Alarme_Clear : Blokta oluşan alarmları silmek için Plus verilmelidir.
Home_Request : Belirtilen pnömatik veya hidrolik pistonun Park Pozisyonuna Alır.
Sns_Work: pistonun çalışma pozisyon sensörüdür. piston çalışma pozsiyonunda ise true olmalıdır.
Sns_Park: Pistonun home vey park pozisyon sensörüdür. piston home pozisyonunda ise true olmalıdır.
Man_Work: Manuel modda çalışma pozisyonuna göndermek için kullanılır.
Man_Park: Manuel modda park(home) Pozisyonunda göndermek için kullanılır.
Auto_Work: Otomatik modda çalışma pozisyonuna göndermek için kullanılır.
Auto_Park: Otomatik  modda park(home) Pozisyonunda göndermek için kullanılır.
T_P_Work: piston üzeride bulunan çalışma pozisyonunda sensörünün pozitif kenar stabil olma süresidir. 
T_P_Park: piston üzeride bulunan Park(Home) pozisyonunda sensörünün pozitif kenar stabil olma süresidir. 
T_N_Work: piston üzeride bulunan çalışma pozisyonunda sensörünün Negatif kenar stabil olma süresidir. 
T_N_Park: piston üzeride bulunan Park(Home) pozisyonunda sensörünün Negatif kenar stabil olma süresidir.
T_Alarm_Work: Piston  Çalışma pozisyonuna gönderildikten sonra çalışma pozisyon sensörünün algılaması için verilen süredir bu süre dolduğunda piston çalışma pozisyon alarm verir.
T_Alarm_Park: Piston  Park(Home) pozisyonuna gönderildikten sonra  Park(Home) pozisyon sensörünün algılaması için verilen süredir bu süre dolduğunda piston  Park(Home) pozisyon alarm verir.
T_Alarm_Park: Piston çalışma veya park(Home) pozisyonuna gönderildiğinde veya gönderilmediğinde herhangi bir sensörden sinyal kesilmesi durumunda Bu parametredeki süre sonunda Alarm_Sns hatası verir.
Valve_Type: 1 ise tek bobinli bir piston içindir 2 çift bobinli pistonlar içindir.
Set_Out: Valfin Çıkışını Setlemek için kullanılır. setlenmediği durumunda false olduğunda gönderilen pozisyonun pozisyon sensörü algılanana kadar çıkış verir true olması durumda gönderilen pozisyonun pozisyon sensörü algılasa bile çıkış vermeye devam eder.
Work_Permit: Çalışma Pozisyonuna göndermek için gerekli olan şartlar bu bölüme girilir ve sistemde istenilmeyen durumlardan korunur.
Park_Permit: Park(Home) Pozisyonuna göndermek için gerekli olan şartlar bu bölüme girilir ve sistemde istenilmeyen durumlardan korunur.
Safety: Çıkışların güvenliğini sağlar çıkış vermesi için true olmalıdır.
Alarm_Close: fonksiyon alarmlarını kapatmak için true yapılır.
INPUT-OUTPUT
Work_Cycle: Blokta çalışma pozisyonu sayar pistonun kaç defa çalışma pozisyonuna gittiği bilgisini verir.
Park_Cycle: Blokta park(Home) pozisyonu sayar pistonun kaç defa park(Home) pozisyonuna gittiği bilgisini verir.
OUTPUT
Q_Work:Valfin Çalışma Çıkışını Verir.
Q_Park:Valfin park(Home) Çıkışını Verir.
Out_Park_Sns: Park Sensörünün Stabilizasyon sürelerinin aktif olduğu çıkıştır.
Out_Work_Sns: Çalışma Pozisyonu Sensörünün Stabilizasyon sürelerinin aktif olduğu çıkıştır.
Move_Order: Çalışma veya park konumuna gönderildiğinde fonksiyon hareket için emir aldığında true çıkışı verir.
Alarm_Work: Çalışma Pozisyonu Hatasının Çıkışı
Alarm_Park: Park Pozisyonu Hatasının Çıkışı
Alarm_Sns: Çalışma ve Park Pozisyonu Hatasının Çıkışı


