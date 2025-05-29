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

- دمج البيانات من المصادر الثلاثة في إطار واحد
- معالجة القيم المفقودة والمكررة
- تحويل أنواع البيانات بشكل مناسب

**English**:

- Merged all data sources into unified DataFrame
- Handled missing values and duplicates
- Proper data type conversions

### 2. التحليل الاستكشافي | EDA

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

يقترح النظام الحلقات بناء على:

معايير التوصية:

- المعيار ١: التوصية بالحلقة الأكثر استماعًا ضمن الفئات التي تفاعل معها المستخدم سابقًا.
- المعيار ٢: التوصية بالحلقة الأكثر استماعًا بين المستخدمين من نفس الجنس.
- المعيار ٣: التوصية بالحلقة الأكثر استماعًا في بلد المستخدم.

* القيود:

- يجب أن تكون الحلقات الموصى بها فريدة.
- يجب ألا يكون المستخدم قد استمع إلى الحلقات الموصى بها من قبل.

Recommends episodes based on:
Recommendation Criteria :

- Criterion 1 : Recommend the most listened-to episode in categories the user has already interacted with.
- Criterion 2 : Recommend the most listened-to episode among users of the same gender.
- Criterion 3 : Recommend the most listened-to episode in the user's country.

* Constraints :

- The recommended episodes must be unique.
- The recommended episodes must not have been listened to by the user before.

## 📝 التوصيات | Recommendations

### 🎤 تحسين المحتوى | Content Improvement

- زيادة إنتاج حلقات "المجتمع" و"الرياضة"
- تحسين جودة حلقات التكنولوجيا (الأقل استماعًا)
- إضافة فقرات قصيرة لجذب الانتباه

- Produce more Society/Sports content
- Enhance Technology episode quality
- Add short attention-grabbing segments

### 💡 تحسين التجربة | UX Enhancements

- نظام توصيات شخصية
- إشعارات للحلقات الجديدة
- ميزة "استكمل الاستماع"

- Personalized recommendation engine
- New episode notifications
- "Continue listening" feature
