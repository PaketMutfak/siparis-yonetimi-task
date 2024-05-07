### Paket Mutfak Sipariş Yönetimi Arayüz Geliştirme Task'ı
![You're finally awake](yourefinallyawake.png)

Merhaba, Paket Mutfak'ın muhteşem sipariş yönetim arayüzünü geliştirme görevine hoş geldiniz! \
Buradaki göreviniz, ~~kasabayı ejderlerden temizlemek~~ Paket Mutfak'ın sipariş yönetimi deneyimindeki bir arayüzü yeniden oluşturmak
 
 Bu görevde React'ı ile ve dilersen Ant Design ve React Query gibi harika araçları kullanarak sipariş yönetimi paneli oluşturacağız.

#### Sözlük

- Sipariş (Order): İçerisinde birden fazla ürün bulunan, teslim adresi ve sipariş saati bilgilerini içeren bir veri modeli.

Siparişler, Hazırlanıyor, Hazırlandı, Yolda ve Teslim Edildi durumlarına sahip olabilir.
- Sepet (Basket): Dağıtılacak bir veya birden fazla siparişin oluşturduğu ve kuryeye atanması gereken siparişlerin bulunduğu veri modeli.

Sepetler, Hazır, Yolda ve Tamamlandı durumlarına sahip olabilir.

- Kurye (Courier): Sepetleri alıp müşterilere siparişleri dağıtan kuryeleri tutan veri modeli.

#### Mockup 

Geliştireceğiniz arayüzü drawio üzerinde [görüntüleyebilirsiniz](https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1&title=ui-drawio.xml#R7Z1td6I4FMc%2FjWdftYcAgr60jztnO7ud2j073Td7KERlisZBnOp8%2BiUKKiSxiTxd2rEv1ICIvxtu7s39k3aMy%2BnqNnTmk8%2FEw0FH17xVx7jq6Dqyeyh%2Boi3rbYuF7G3DOPS9ZKd9w9D%2FiZNGLWld%2Bh5eZHaMCAkif55tdMlsht0o0%2BaEIXnN7jYiQfZb584YMw1D1wnY1n98L5psW3u6vW%2F%2FHfvjSfrNyOpvt0yddOfklywmjkdeD5qM645xGRISbV9NV5c4oPBSLtvP3Qi27k4sxLNI5gM%2Fv98O7qe%2B%2F%2F3my3%2F3g%2BHDYPVldaZvj%2FLDCZbJD05ONlqnBEKynHmYHkTrGBevEz%2FCw7nj0q2vsc3jtkk0DeJ3KH7JnlRynj9wGOHVQVNykreYTHEUruNdkq1dLQGW9BjdSN6%2F7vl3raRtcsjeSludxOjj3cH3XOIXCRoVTNrbnMYxqLn87991Wec5PYJ2nIuZ42JzuBgcLjug5WNBDJahH%2F94f4Hp1%2FkRvfD9MQ7j52c%2FGPsBfVlu%2Fzpur7d73QE90%2Bb1qurosRdf6%2BglfRGZbF%2Bsm6bxbmjyruy6aZoimnHjn6RjDOJnxPCLf2CUheQE%2FngWv3ZjSDFw44Ji8OPxdZBsmPqeRz%2FOpZ21R%2FnA061Zz4pY%2FLzxxqgMflcCPjsAvRP43abpWxL0jXdKX%2B91G6bfY%2BhD89LJ1t1H1rn3h%2FGYzmG3c%2BWlwzNZr30EHnob3sgPgksSkHDzWWPUc7Hrxu2LKCQv%2BGDLc69rdivtqGYONy%2FkqHeMNFhHwdAWJAVqTNRTBTZ8SK%2FrzEVcWUc0bJEPbTgY29lMLTHQ6u1YrA9sHb1jiUHNNPvvhiY3MaiXZmrPNiYGCsBhJgamcL4FfmJQHH7TiYEpnK%2BBnxgUpt94YmCySfERLy0R21ZGzkTdLDqO1643UjXZubFi7HJ5gdfFPc%2Fk5QU9%2FdmwrFpoN0a3yw6JDN3FC47cSXLNHrqCxXxbtRr5Kwo%2FR3BGZtQN7EpHGsveuOhd3SCOE4kINVrgPOPgniz8yCdcn3OX2%2BGZRBGZbr90Ts9%2BuhrT0t752J3r5%2B4Euy%2FV2dLIXjkGa1rDPudlMpXZlh1xWdvmQE2J%2B7Kcn0%2BdkD6F2PvKyaRHWvzI9oWMlXkXILdvVGeMXL0J2aw1eNMb1Y0A0vk2i7tL%2F2g7mUWHF8%2FmwXNc1uZRwoSGcvKen1cy%2BpLzSpVVP002mz8yfEgkSCLriK0gspukdcyT0v6aKfNmPq0gSn79piOlAKzvSyobiH%2B%2BoW0eh03WmD7%2F8ffD03X8oUF6kPiktsfZbmcsWG2cSr86UXfoJmvQm82jEoOmW3v5dIK5qlCtAa0lETbUrSmwLY6vqVdTYEHVFFgiDw9JU2AJc9T20IOjKbCgagrUaQLQFFgt1hQoAIc5dWi1WFNQHH7TU4dWizUFhek3PnVolZ2%2FVEYOoKYg1TOXVeUWQmlflTs9MLzwoC9gDKnKbYMN9OXpwaly22ADf2WaAKrctjDwb0GoKg8cZqhqy%2BQJUEPVwvCbDlVtmUQBaqhalH7joaotUeOoosqtTg5elRtpEtphpVBVBEU5VG2%2BSG0r5UBNSgD2ZlSKXmvGKdHVPmLNX8V4ydZ8ubPxmj%2BqWi5Tnoy%2BFdcKkrktoRUiilN695uKllo1FAixeSK0MRJOQIFao5vb2xWyI0AyjuAjjpoK1oM6aqbyCpDqrPImneGps3rsPOoRJwVRndUTWQeQOqvHGzeLq7Mu36U6S8GgUNVZSANb94J3JyxCEs4fSKCkyc90NchTRnb%2BEQMlBetBDZQQkriTqW7hJ9I5dYealZ8ICVUyDdcw9yaDrP1ECOpd9yr84Kg%2FEYJ6H%2F4JPAHoPxES3onfAV9VV0EOs6yOOIsYtqauXgL%2BpgvrSLxaYgd8Zb04%2F8ZL6ygNs%2BqWgZ7ADqAOFHEWWGTwqSTEYiztU4Ii8XqJTYcKO7NB1oIi8ZKHLeIHRw2KxIsYto8nAD0o0oWpVQtCVwXkUENXYSbWgtC1OP7mQ1eZzA1q6FqYf%2FOha3rkumWhJ7ADKOMwJGbTlSJXIZUWCkORoZQWNVq7MUTz35BqN4ZEnvQhazcK1gNbuzEkFExNuxJAjrfsNfsqdC2mwA6gXIvE3SEf07XIWw%2Bua5G4Q6MxAV2Jk3XwFHSIs%2BD2ET8FUUK37z2ANXSIsxT3ryXOyjApWBUdZ7nwYvFSeX4IoIyOs7431HhpZ1jI8RJnxe5f8ZKi9cDGS9wFwTODyd7K6chBN5wtNj6azlia1ny1HU9yI8vw0%2F3g4dMw3uXq%2BnHwFD9%2F%2FutqcPfbJ9mRpuBknHKmfLYDnWZ%2FGiesQvyyCarQSBaDBntjPEzekjCakDGZOcH1vjU3rO73uSP0wtkg%2B4ajaJ0Mts4yIpJAF2QZuvjICaeTYZETjvHxSyjpfvTnHLVQiAMn8n%2FgzIlUQNpugnQMOFx%2FpZ8%2F76Zvn5LDbd5crTLv1h3R3L2shXalTcgm8j3jcbmYfbu565t9v780Rw%2F%2Fcv7X7gV%2BCfAaz%2BLWpJzCK8PWFrUa%2FADgBGfUz8ehrC%2FSeeLiMhwRl%2F3p2pXSJNdn%2BQXVdZ6op%2BZ%2FbFzXvWNlTEwcNaxa2lszZaV%2Fy3eS1qIgG36QJys6291MUH73PP0mLCUi6sljlhQn1uKKq6tToIGVqp90u1XNynShuqE98ADdNiGUmbeOJoSbJmSWY4MqPCu6HFvjujOZZZvZEemdwG9cdSajuYQqOitKv3HNGUfyx6CGEHpZsiNehf%2FtGOqIp7ch%2BOKo81pHD070xVHztZUmgOiLo%2BVrTfSlABxm9MXR2rUm%2BioOv%2Bnoi6Pda030VZh%2B49GX0jLQ6vOynoN7I%2B4KpJbbw8%2BjCucYu1mVqsmbOjM5qCubnGWzjFRX1B4BUTmmQbmyTVerUT%2FE%2FQmc0PD6%2FvqxgUF3Y5vky1DOVlVOyeeyHU6AiXg1%2FcosIlHKEK3G6zmLyY6nvG3yahcnDMnrQt8%2B08NuasrntGbkUWgmPfyM7EU9rGmUK5r5K8PmhKb8AaJblSFYt%2FVEAs958Tvvq5hsMZrG6mrJ8duQUCHQbtst7XKfiYfpHv8D) \
 


#### Projenin başlatılmasına dair notlar
- Projeyi React ile hazırlamalısınız.\
- Ant design ve React Query kullanmanızı bekliyoruz, ancak başka bir tercihlerde bulunabilirsiniz.\
db.json verisini json-server ile çalıştırmalısınız. Json Server'a uygun istekler geliştirmenizi bekliyoruz.\
- Daha iyi bir veri modeli fikrim var derseniz veriyi de değiştirebilirsiniz.


#### Beklentiler
2 adet sipariş yönetim sütunu olması bekleniyor: **Bekleyen Siparişler** ve **Yoldaki Siparişler**.\
1. İlk sütün "Bekleyen Siparişler" hazırlanmış siparişleri ve yola çıkmaya hazır sepetleri gösterecek.\
    Üst tarafta sepetleri, alt tarafta herhangi bir sepete atanmamış, hazırlanmış siparişleri gösterecek.\
    Siparişlerin sepetlere atanmasını ve sepetlerden çıkarılmasını bekliyoruz.\
    Burada sepet oluşturma deneyimini senden bekliyoruz.\
    Örneğin iki siparişi birbirinin üstüne atıp bir sepet oluşturabilirsin ve bu sepete daha fazla sipariş atabilirsin. Ya da bu siparişlerin üstünde "checkler" oluşturup bir buton yardımıyla sepet oluşturabilirsin. Burada yazdıklarımızdan bağımsız kendi düşündüğün bir deneyimi de bize sunabilirsin.\
    Sepet'e bir kurye atanmalı.\
    İçerisindeki siparişler ve kuryeler atanmış bir sepeti tercihen drag and drop ya da başka bir yöntemle sağdaki Yoldaki Siparişler sütununa geçirebilmeli.\
    Kuryesi atanmamış bir Sepet Yoldaki Siparişler sütununa geçememeli.

2. İkinci sütun “Yoldaki Siparişler”e geçen sepetleri gösterecek.\
    Bu sepetlerin kuryesi ve içerisindeki siparişler değiştirilememeli.\
    Bir sepetin içerisindeki siparişler “Teslim Edildi”, ve “Teslim Edilemedi” butonları olmalı. ❌, ✅ şeklinde olabilir.\
    Yoldaki Siparişler sütunundaki sepetteki siparişlerin “Teslim Edildi” veya “Teslim Edilemedi” olarak işaretlenenler bir şekilde belli olmalı.\
    Tüm siparişleri “Teslim Edildi” işaretlenen bir sepet bu sütundan silinmeli.

#### Ekstra Notlar
Beklentilerin herhangi bir satırında daha iyi bir fikriniz varsa bu fikri uygulayabilirsiniz.\
Kullanıcı deneyimini iyileştirmekte özgürsünüz.\
Ekstra olarak tamamlanmış sepetler sütunu oluşturup içerisini dilediğiniz gibi tamamlayabilirsiniz.\
Siparişlerin içeriğini görüntüleyebilmek için bir Sipariş Detayı Modalı oluşturup içeriğini dilediğiniz gibi oluşturabilirsiniz.\
Mikro interaksiyonlara önem veriyoruz.\
Zamanınıza hepsinden daha çok değer veriyoruz. Bu task gereğinden fazla zamanınızı alıyorsa yapabildiğiniz kadarını yapıp bize iletebilirsiniz.\
Yazdığınız kodu çektiğimizde nasıl çalıştırmamız gerektiğine dair kısa bir README yazabilirsiniz.