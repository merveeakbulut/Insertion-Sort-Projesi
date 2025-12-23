# Insertion Sort Projesi

## Proje 1
**Dizi:** `[22, 27, 16, 2, 18, 6]`

### 1. Yukarı verilen dizinin sort türüne göre aşamaları

Insertion Sort (Araya Ekleme Sıralaması), her adımda sıradaki elemanı solundaki sıralı kısmın içine uygun yere yerleştirir.

* **Başlangıç:** `[22, 27, 16, 2, 18, 6]` (22 sıralı kabul edilir).
* **Adım 1:** 27 sayısı 22'den büyüktür, yeri değişmez.
    * `[22, 27, 16, 2, 18, 6]`
* **Adım 2:** 16 sayısı 27 ve 22'den küçüktür, en başa gelir.
    * `[16, 22, 27, 2, 18, 6]`
* **Adım 3:** 2 sayısı hepsinden küçüktür, en başa gelir.
    * `[2, 16, 22, 27, 18, 6]`
* **Adım 4:** 18 sayısı 22'den küçük, 16'dan büyüktür. Araya girer.
    * `[2, 16, 18, 22, 27, 6]`
* **Adım 5:** 6 sayısı 16'dan küçük, 2'den büyüktür. Araya girer.
    * **Sonuç:** `[2, 6, 16, 18, 22, 27]`

### 2. Big-O Gösterimi
Insertion Sort algoritmasının Time Complexity (Zaman Karmaşıklığı) değeri: **O(n²)**

### 3. Time Complexity Case (18 Sayısı)
Dizi sıralandıktan sonraki hali: `[2, 6, 16, 18, 22, 27]`

Aradığımız sayı **18**, dizinin tam ortasında yer almaktadır. Bu nedenle **Average Case (Ortalama Durum)** kapsamına girer.

* **Best Case:** Aranan sayı en başta (2) olsaydı.
* **Worst Case:** Aranan sayı en sonda (27) olsaydı.
* **Average Case:** Aranan sayı ortada (18) olduğu için bu kapsama girer.

---

## Proje 2 (Selection Sort)
**Dizi:** `[7, 3, 5, 8, 2, 9, 4, 15, 6]`

Selection Sort (Seçmeli Sıralama), dizideki en küçük elemanı bulup en baştakiyle değiştirerek ilerler.

**İlk 4 Adım:**

* **1. Adım:** Dizideki en küçük sayı **2**'dir. En baştaki 7 ile yer değiştirir.
    * `[2, 3, 5, 8, 7, 9, 4, 15, 6]`
* **2. Adım:** Kalan kısımdaki (3'ten itibaren) en küçük sayı **3**'tür. Zaten 2. sıradadır, yeri değişmez.
    * `[2, 3, 5, 8, 7, 9, 4, 15, 6]`
* **3. Adım:** Kalan kısımdaki (5'ten itibaren) en küçük sayı **4**'tür. 3. sıradaki 5 ile yer değiştirir.
    * `[2, 3, 4, 8, 7, 9, 5, 15, 6]`
* **4. Adım:** Kalan kısımdaki (8'den itibaren) en küçük sayı **5**'tir. 4. sıradaki 8 ile yer değiştirir.
    * `[2, 3, 4, 5, 7, 9, 8, 15, 6]`
