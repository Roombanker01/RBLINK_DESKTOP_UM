# Hub ayrıntıları

## Koruma ve günlükler

**Disarm**, **Arm Stay** ve **Arm Away** birbirini dışlar. Hedef Hub'ı doğrulayın, bir standart durum seçin ve yenilenen durumu sonuç kabul edin. Özel savunma bölgeleri ayrıdır: yönetici tanımlı adlarla en fazla sekiz bölge bağımsız etkinleştirilebilir veya kapatılabilir. Bu güvenlik açısından hassas işlemlerde ayrılmadan önce Hub'ı ve yenilenen durumu doğrulayın.

On günlük zaten varsa **Get Log** engellenir ve önce eski günlük silmeniz istenir. Kullanılabilir günlükte **Download** doğrudan başlar. İstek veya silme sonucunu yenilenen listeden doğrulayın.

![Standart Hub koruma onayı: 1 sonuç](/images/hubs/hub-standard-arm-confirm.png){.manual-shot}

| No. | Denetim | Sonuç veya risk |
|---|---|---|
| 1 | Onay iletisi | Seçilen standart modu ve hedef Hub'ı doğrulayın. |
| 2 | İptal | Korumayı değiştirmeden kapatır. |
| 3 | Onayla | Seçilen standart koruma değişikliğini gönderir. |

![Özel Hub savunması onayı: 1 sonuç](/images/hubs/hub-custom-defence-confirm.png){.manual-shot}

| No. | Denetim | Sonuç veya risk |
|---|---|---|
| 1 | Onay iletisi | Adlandırılmış özel bölgeyi ve hedef Hub'ı doğrulayın. |
| 2 | İptal | Özel savunmayı değiştirmeden kapatır. |
| 3 | Onayla | Seçilen özel savunma değişikliğini gönderir. |

![Hub günlük sınırı uyarısı: 1 uyarı](/images/hubs/hub-log-limit-warning.png){.manual-shot}

| No. | Denetim | Sonuç |
|---|---|---|
| 1 | Get Log | On günlük sınırında istek yeni günlük oluşturmaz. |
| 2 | Uyarı iletisi | Yeni günlük istemeden önce eski günlüğü silin. |

![Hub ayrıntıları: 1 Hub Listesi, 2 Hub Ayrıntısı, 3 Uzak yapılandırma, 4 Alt cihazlar, 5 Alt cihaz ekle, 6 Düzenle, 7 Disarm, 8 Arm Stay, 9 Arm Away, 10 Perimeter, 11 Night Watch](/images/hubs/hub-detail-main.png){.manual-shot}

| No. | Denetim | Ön koşul, işlem, sonuç, hata veya izin |
|---|---|---|
| 1 | Hub Listesi | Hub listesine döner. |
| 2 | Hub Ayrıntısı | Seçili Hub’ın adını, SN’sini, sahipliğini, durumunu ve mevcut denetimleri gösterir. |
| 3 | Uzak yapılandırma | Seçili Hub yapılandırmasını açar. Kullanıcı, SSH ve yeniden başlatma denetimleri role bağlıdır. |
| 4 | Alt cihazlar | Alt cihaz listesini açar; fiziksel cihaz kaldırmaz. |
| 5 | Alt cihaz ekle | Alt cihaz kaydını açar. |
| 6 | Düzenle | Yetkili kullanıcı Hub adını veya şirket atamasını değiştirir; reddedilen istek önceki atamayı korur. |
| 7 | Disarm | Seçili Hub için devre dışı bırakma onayını açar. |
| 8 | Arm Stay | Seçili Hub için Arm Stay onayını açar. |
| 9 | Arm Away | Seçili Hub için Arm Away onayını açar. |
| 10 | Perimeter | Etkinse yapılandırılmış Perimeter özel savunmasını seçer. |
| 11 | Night Watch | Etkinse yapılandırılmış Night Watch özel savunmasını seçer. |

![Hub günlükleri: 1 İndir, 2 Sil, 3 Günlük al, 4 Mesajları Excel’e aktar, 5 Listeye dön](/images/hubs/hub-detail-logs.png){.manual-shot}

| No. | Günlük veya dışa aktarma denetimi | Ön koşul, işlem, sonuç, hata veya izin |
|---|---|---|
| 1 | İndir | Mevcut seçili günlüğü indirir. Eksik indirme bilgisi veya yetki hatası Hub sahipliğini değiştirmeden hata verir. |
| 2 | Sil | Seçili günlük için silme onayını açar; onaylanana kadar silmez. |
| 3 | Günlük al | Hub’dan günlükleri toplar ve başarı sonrası listeyi yeniler; hata listeyi değiştirmez. |
| 4 | Mesajları Excel’e aktar | Bu Hub mesajları için dışa aktarma isteği yollar; hata Hub ve günlük kayıtlarını değiştirmez. |
| 5 | Listeye dön | Hub listesine döner. |

![Hub günlüğü silme onayı: 1 uyarı, 2 İptal, 3 Tamam](/images/hubs/hub-log-delete-confirm.png){.manual-shot}

| No. | Onay denetimi | Kullanım ve risk |
|---|---|---|
| 1 | Uyarı | Devamdan önce gösterilen günlüğün amaçlanan kayıt olduğunu denetleyin. |
| 2 | İptal | Günlüğü silmeden iletişim kutusunu kapatır. |
| 3 | Tamam | Başarılı yetkili istekten sonra yalnızca seçili günlüğü siler; Hub bağını, fiziksel SN’yi veya alt cihazları silmez. |
