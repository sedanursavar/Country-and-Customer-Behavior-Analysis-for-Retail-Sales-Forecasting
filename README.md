# Country-and-Customer-Behavior-Analysis-for-Retail-Sales-Forecasting
( Perakende Satış Tahmini için Ülke ve Müşteri Davranışı Analizi)
**PROJENİN AMACI**
Yapılan proje ile Online Retail adlı bir datasetle hem gözetimli hem gözetimsiz öğrenme ile müşteri davranışlarını anlamak ve bu doğrultuda Regresyon algoritması ile toplam satış miktarı hakkında tahminde bulunmak amaçlanmıştır.
Alınan satış tahminleri envanter yönetimi ve talep planması hakkında fikir verecektir. Bu tahminler müşteri davranışlarını anlamak ve gelecekteki satışları tahmin etmeye yaradığından işletmelerin stok yönetimi ,pazarlama stratejileri ve genel iş planlamasını optimize etmeye yarar.

**VERİ SETİ**
541909 satırdan oluşmaktadır.Sütun isimler ise aağıdaki gibidir:
Invoice no: Satın alınan ürünün fatura numarası.
StokCode: Satın alınan ürünü tanımlamak için kullanılan bir kod
Description: Satın alınan ürünün kısa açıklaması.
Quantity: Satın alınan ürünün miktarı
InvoiceDate: Satın alma işleminin gerçekleştiği tarih ve saat 
UnitPrice: Satın alınan ürünün bir biriminin fiyatı
CustomerId: Satın alma işlemini gerçeşkleştiren müşteriye ait benzersiz bir tanımlayıcı
Country: Satın alma işlemini gerçekleştiren müşterinin bulunduğu ülke 

**DEĞİŞKENLER**
Hedef değişken: TotalSales=UnitPrice*Quantity 
Toplam satışı bulmaya yarayan bir değişken oluşturulup devam edilmiştir. Diğer tüm değişkenler yardımcı değişken olarak belirlenmiştir.

**KULLANILAN KÜTÜPHANELER**
import pandas as pd --> Verileri işlemek için kullanılmıştır.
import numpy as np --> Sayısal hesaplamalar için kullanılmıştır.
import matplotlib.pyplot as plt --> Veri görselleştirme için kullanılmıştır. Grafik ve çizimler için
import seaborn as sns --> Daha gelişmiş bir veri görselleştirme için kullanılmıştır. 
from sklearn.model_selection import train_test_split, GridSearchCV--> Hiperparametre optimizasyonu için kullanılmıştır. Modeli değerlendirip en iyi sonucu almak için kullanılmıştır
from sklearn.ensemble import RandomForestRegressor -->Veri ilişkisini modellemek için kullanılmıştır.   Bir regresyon modeli olup karar ağaçlarını kullanarak tahminler yapar
from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score-->
from sklearn.preprocessing import StandardScaler-->
import warnings
warnings.filterwarnings("ignore", category=FutureWarning)-->
import plotly.express as px-->Etkileşimli ve dinamik grafikler için.

**MODEL PERFORMANSI ÖLÇÜMÜ**
MAE (Mean Absolute Error): Hata değerlerinin mutlak ortalaması.
MSE (Mean Squared Error): Hata karelerinin ortalaması.
RMSE (Root Mean Squared Error): MSE'nin karekökü, daha sezgisel bir hata metriği.
R² Skoru: Modelin ne kadar iyi bir şekilde tahmin yaptığını gösteren bir metriktir.

---Projede kullanılan çeşitli grafikler de projeyi daha iyi yorumlamamıza yardımcı oldu.
**SONUÇ**
Kulladığımız veri kümeleri ile satıl tahmini yapmak üzere gözetimli ve gözetimsiz olmak üzere iki öğrenme modeli geliştirildi. Gözetimsiz öğrenme ile yapılan projenin daha başarısız olduğu gözlemlendi.

https://www.kaggle.com/code/sedanursavar/notebookf437ef569e/notebook?scriptVersionId=197349778



