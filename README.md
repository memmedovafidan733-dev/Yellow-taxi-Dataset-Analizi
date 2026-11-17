# Yellow-taxi-Dataset-Analizi
Yellow Taxi datası ilə həftəlik gedişlərin və sürücülərin analizi. 

## Xülasə
Bu layihə 13-19 fevral 2023-cü il tarixlərində gecə saatlarında edilmiş 4637 taksi sifarişindən ibarət həftəlik data üzərindən analizi əhatə edir.


## Layihənin məqsədi
* Sürücülərin aktiv qalma müddəti, ümumi gediş və müştəri sayı, gəlirinə əsasən kateqoriyalara bölünməsi;

* Kateqoriyalarına əsasən sürücülər üçün bonus sisteminin tətbiqi və növbəti həftəlik planın təyin edilməsi;

* Müştərilərin taksi xidmətindən istifadə sıxlığına əsasən fərdi endirim kampaniyalarının tətbiqi;

* Gediş məsafəsi aralıqları üzrə gediş sayları anomaliyasının tapılması (Outlier analizi).


### Layihədə istifadə edilən texniki alətlər
    Microsoft Excel   •   Power Query   •   Power Pivot   •   Pivot Table


### Faylın strukturu (Excel workbook)
1. "Yellow taxi 13-19 February 2023" adlı səhifə - İlkin dataset.  
2. "Taxi data query" adlı səhifə - Power Query ilə transformasiya edilmiş əsas cədvəl.  
3. "Aktiv qalma müddəti" adlı səhifə - Sürücülərin tarixlər üzrə gündəlik və orta günlük aktiv qalma müddəti üzrə cədvəl (saat olaraq).  
4. "Reyting-Bonus-Plan" adlı səhifə - Sürücülər üzrə ümumi gediş sayı, ümumi müştəri sayı, ümumi gəlir kimi göstəricilər, reytinq kateqoriyası üzrə bölgü, kateqoriyalara əsasən bonus və növbəti həftəlik plan hədəfləri üzrə cədvəl.  
5. "Kampaniya" adlı səhifə - Müştərilərin günlük orta gediş sayı və günlük orta gediş məsafəsinə əsasən növbəti həftə üzrə tətbiq ediləcək kampaniyalar üzrə cədvəl.  
6. "Outliers" adlı səhifə - Qruplaşdırılmış gediş məsafəsi(trip distance) intervalı üzrə hər sürücünün yerinə yetirdiyi sifariş sayına əsasən outlier dəyərlərə malik sürücülərin məlumatlarının aşkarlanması.


### Layihədə icra edilən proseslər
* Power Query: Tarix sütununun Split Column vasitəsilə ayrılması;  
* Power Pivot: Göstəricilərin, reytinq kateqoriya bölgüsünün, növbəti həftəlik planın və endirim kampaniyalarının hesablanması üçün measures vasitəsilə data modelin qurulması;
* Pivot Table: Nəticələr üzrə ümumiləşdirilərək cədvəl hesabatların hazırlanması;
* İstifadə edilən funksiyalar: IF, AND, OR, MAX, MIN, CALCULATE, SUM, COUNT, SUMX, DISTINCT, SWITCH, DISTINCTCOUNT, ALL, QUARTILE.EXC, IQR metodu ilə outlier dəyərlərin tapılması;
* Conditional formatting: Outlier dəyərlərə malik sürücülərin məlumatlarının şərti formatlama ilə vizuallaşdırılması.


    Şəkil: Power Pivotda yaradılmış göstəricilər
<img width="1913" height="1028" alt="image" src="https://github.com/user-attachments/assets/e5ada8d6-5981-4946-9a61-57032dceb9ce" />
