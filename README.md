# 🎭 NetCoreAI Project 13 - Advanced Sentiment & Emotion Analysis

Bu proje, **.NET Console Application** kullanarak **OpenAI Chat Completions API** üzerinden gelişmiş duygu analizi yapmaktadır.  
Kullanıcıdan alınan metin analiz edilerek şu duyguların yüzdelik skorları çıkarılır: **Joy, Sadness, Anger, Fear, Surprise, Neutral**.  
Sonuç JSON formatında konsola yazdırılır.  

---

## 🛠️ Kullanılan Teknolojiler
- .NET 8 / 9 Console Application  
- OpenAI API (Chat Completions - `gpt-3.5-turbo`)  
- HttpClient (API isteği için)  
- Newtonsoft.Json (JSON serialize/deserialize)  

---

## 📂 Proje Yapısı
- `Program.cs` → Kullanıcıdan metin alır, OpenAI API’ye gönderir, JSON formatında duygu analizi sonucunu döndürür.  
- `.csproj` → Proje yapılandırma dosyası  

---

## ⚙️ Kurulum ve Çalıştırma
1. Repo’yu klonla:
   git clone https://github.com/kullaniciadiniz/NetCoreAI_Project_13_AdvancedSentimentAnalysis.git
   cd NetCoreAI_Project_13_AdvancedSentimentAnalysis
Program.cs içinde kendi OpenAI API anahtarını ekle:
private static readonly string apiKey = "YOUR_API_KEY";

Konsol uygulamasını çalıştır:
dotnet run

Konsolda örnek kullanım:
Bir metin giriniz:
> Bugün çok mutluyum çünkü güzel bir haber aldım.

Gelişmiş duygu analizi yapılıyor...

Sonuç:
{
  "Joy": "85%",
  "Sadness": "5%",
  "Anger": "0%",
  "Fear": "2%",
  "Surprise": "8%",
  "Neutral": "0%"
}
✨ Özellikler
✔️ Kullanıcıdan metin alır

✔️ OpenAI API ile duyguları yüzdelik değerlere ayırır

✔️ JSON formatında çıktı döndürür

✔️ 6 farklı duygu kategorisini (Joy, Sadness, Anger, Fear, Surprise, Neutral) analiz eder

﻿
