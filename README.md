# مشروع ثمانية - تحليل بيانات البودكاست ونظام التوصيات  
# Thamena Project - Podcast Data Analysis & Recommendation System

 ## 📌 نظرة عامة | Overview
 
يهدف هذا المشروع إلى تحليل بيانات مستمعي منصة "ثمانية" للبودكاست لفهم أنماط الاستماع وتقديم توصيات لتحسين المحتوى وتجربة المستخدم.

This project analyzes listener data from Thamena podcast platform to understand listening patterns and provide content improvement recommendations.

## 📂 مصادر البيانات | Data Sources
تم استخدام ثلاث مجموعات بيانات رئيسية:
- **users.csv**: بيانات ديموغرافية (العمر، الجنس، الدولة)
- **episodes.csv**: تفاصيل الحلقات (العنوان، التصنيف)
- **listens.json**: سجلات الاستماع (المدة، التكرار)

Three core datasets were used:
1. `users.csv`: Demographic data (age, gender, country)
2. `episodes.csv`: Episode details (title, category)  
3. `listens.json`: Listening records (duration, frequency)

## 🔍 منهجية التحليل | Analysis Approach

### 1. تنظيف البيانات | Data Cleaning
**عربي**:  
- دمج البيانات من المصادر الثلاثة في إطار واحد
- معالجة القيم المفقودة والمكررة
- تحويل أنواع البيانات بشكل مناسب

**English**:  
- Merged all data sources into unified DataFrame
- Handled missing values and duplicates
- Proper data type conversions

### 2. التحليل الاستكشافي | EDA
**عربي**:  
- تحليل توزيع الأعمار والجنسيات
- تحديد أكثر الفئات شعبية
- حساب متوسط مدة الاستماع
- مقارنة أنماط الاستماع بين الجنسين

**English**:  
- Age and gender distribution analysis
- Most popular category identification  
- Average listening duration calculation
- Gender-based listening pattern comparison



## 🚀 نظام التوصيات | Recommendation System

### 📌 المنطق | Logic
**عربي**:  
يقترح النظام الحلقات بناء على:
1. تاريخ الاستماع السابق
2. التفضيلات الديموغرافية
3. شعبية المحتوى

**English**:  
Recommends episodes based on:
1. Listening history
2. Demographic preferences  
3. Content popularity

## 📝 التوصيات | Recommendations

### 🎤 تحسين المحتوى | Content Improvement
**عربي**:  
- زيادة إنتاج حلقات "المجتمع" و"الرياضة"
- تحسين جودة حلقات التكنولوجيا (الأقل استماعًا)
- إضافة فقرات قصيرة لجذب الانتباه

**English**:  
- Produce more Society/Sports content  
- Enhance Technology episode quality
- Add short attention-grabbing segments

### 💡 تحسين التجربة | UX Enhancements
**عربي**:  
- نظام توصيات شخصية
- إشعارات للحلقات الجديدة
- ميزة "استكمل الاستماع"

**English**:  
- Personalized recommendation engine
- New episode notifications  
- "Continue listening" feature


