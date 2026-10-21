FBN Office Accounts Android App — সহজ নির্দেশনা

এই ZIP-এ Android অ্যাপের SOURCE PROJECT আছে, তৈরি APK ফাইল নেই।
এটি আপনার Google Apps Script FBN Office Accounts লিংক WebView-তে খোলে।
আপনার Google Sheets ডেটা বা Apps Script কোড পরিবর্তন করে না।

সবচেয়ে সহজে APK বানানোর বিকল্প (কম্পিউটারে Android Studio ছাড়াই):
1. https://github.com/ এ সাইন ইন/অ্যাকাউন্ট খুলুন।
2. New repository তৈরি করুন; নাম দিন fbn-office-accounts-android।
3. ZIP ফাইলটি নিজের কম্পিউটারে Extract করুন।
4. GitHub repository-তে Add file > Upload files নির্বাচন করে Extract করা ফোল্ডারের সব ফাইল/ফোল্ডার আপলোড করুন।
   .github ফোল্ডারটিও আপলোড করতে হবে। GitHub যদি লুকানো ফোল্ডার না দেখায়, তাহলে GitHub Desktop ব্যবহার করা সহজ হতে পারে।
5. Commit changes করুন।
6. Repository-এর Actions ট্যাবে যান। “Build FBN Android APK” workflow চালু/দেখুন।
7. Workflow সবুজ (successful) হলে রান খুলুন, নিচে Artifacts অংশ থেকে FBN-Office-Accounts-APK ডাউনলোড করুন।
8. ZIP artifact Extract করলে app-debug.apk পাবেন। সেটি Android ফোনে পাঠিয়ে ইনস্টল করতে পারবেন।
   ফোনে ইনস্টল করার সময় Android অনুমতি চাইতে পারে।

দ্রষ্টব্য:
- GitHub Actions প্রথমবার চালাতে workflow অনুমতি বা Actions enable করতে হতে পারে।
- এই debug APK পরীক্ষার জন্য। Play Store প্রকাশের জন্য আলাদা signed AAB, signing key, privacy/policy প্রস্তুতি এবং Play Console প্রয়োজন।
- Apps Script লগইন/Google sign-in WebView-তে সবসময় কাজ নাও করতে পারে; APK পাওয়ার পর পরীক্ষা করা জরুরি।
- যদি build error আসে, Actions-এর লাল error অংশের screenshot পাঠান।
