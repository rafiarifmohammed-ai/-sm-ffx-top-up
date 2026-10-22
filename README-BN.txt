SM FFX TOP UP — প্রাথমিক প্রজেক্ট

ফাইলসমূহ:
- user.html: কাস্টমার/টপ-আপ পেজ
- admin.html: অ্যাডমিন ড্যাশবোর্ড
- FFX.html: Nickname/অতিরিক্ত পেজ
- account.js: ওয়েবসাইটের নাম ও Telegram/YouTube লিংক
- JPG ফাইল: সাইটের ছবিগুলো

গুরুত্বপূর্ণ: নিরাপত্তার জন্য আগের সাইটের Firebase কনফিগ সরিয়ে YOUR_* placeholder বসানো হয়েছে। নিজের Firebase কনফিগ না বসালে লগইন/ডেটাবেস কাজ করবে না।

সেটআপ:
1. Firebase Console-এ নিজের নতুন Project তৈরি করুন।
2. Authentication-এ Email/Password চালু করুন।
3. Firestore Database এবং প্রয়োজন হলে Realtime Database তৈরি করুন।
4. user.html ও admin.html-এ YOUR_* placeholder-গুলোর জায়গায় নিজের Firebase web config বসান। দুই ফাইলেই একই Project ব্যবহার করুন।
5. নিজের admin email দিয়ে Firebase Authentication-এ user তৈরি করুন।
6. Firestore/Realtime Database Rules নিরাপদভাবে সেট করুন—কখনোই production-এ test mode বা সবার read/write access রাখবেন না। Admin page-এর URL গোপন রাখাই যথেষ্ট নয়; database rules দিয়ে admin data সুরক্ষিত করতে হবে।
7. account.js-এ YOUR_CHANNEL_USERNAME, YOUR_GROUP_USERNAME, YOUR_CHANNEL পরিবর্তন করে নিজের লিংক বসান।
8. Firebase rules এবং অর্ডার/পেমেন্ট ফ্লো পরীক্ষা করে তারপর সাইট live করুন।

নোট: এই ফোল্ডারটি ব্র্যান্ডিং-সহ প্রাথমিক রূপ। Firebase কনফিগ, database rules, payment details এবং live deployment এখনো সেটআপ করা হয়নি। bKash/Nagad-এর প্রকৃত payment integration আলাদাভাবে যাচাই করতে হবে।
