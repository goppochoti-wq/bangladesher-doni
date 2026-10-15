বাংলাদেশের ধনী — Android Studio Project

এই প্রজেক্টে Step 162-এর HTML গেমটি Android WebView-এর মধ্যে চালানোর জন্য রাখা হয়েছে।
গেমের HTML ফাইলটি app/src/main/assets/index.html-এ আছে।

APK বানানোর ধাপ:
১. কম্পিউটারে Android Studio ইনস্টল কর।
২. Android Studio-তে Open চাপ দিয়ে এই ফোল্ডারটি খুল:
   Bangladesher_Dhoni_Android_Project
৩. Gradle sync শেষ হওয়া পর্যন্ত অপেক্ষা কর। প্রয়োজন হলে Android SDK Platform 35 ও
   Android Gradle Plugin-এর জন্য ইন্টারনেট লাগতে পারে।
৪. Build > Build Bundle(s) / APK(s) > Build APK(s) নির্বাচন কর।
৫. সফল হলে Android Studio APK-এর অবস্থান দেখাবে; সাধারণত:
   app/build/outputs/apk/debug/app-debug.apk

ফোনে পরীক্ষা:
- APK ফোনে ইনস্টল করে চালাও।
- গেমের সেভ/লোড localStorage ব্যবহার করলে WebView-এর DOM storage চালু আছে।
- প্রথমবার ইনস্টল করার পর সেভ করা গেম Android অ্যাপের নিজস্ব স্টোরেজে থাকবে;
  ব্রাউজারের আগের সেভ স্বয়ংক্রিয়ভাবে স্থানান্তর হবে না।

গুরুত্বপূর্ণ:
- এটি Android Studio-তে বিল্ড করার জন্য সোর্স প্রজেক্ট; APK ফাইল এখনো বিল্ড করা হয়নি।
- এই পরিবেশে Android SDK/Gradle দিয়ে বিল্ড ও ডিভাইস টেস্ট করা হয়নি।
- গেমের HTML ফাইলটি অপরিবর্তিত কপি করা হয়েছে।
