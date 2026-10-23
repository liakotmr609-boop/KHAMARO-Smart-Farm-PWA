KHAMARO Smart Farm — প্রথম PWA প্রোটোটাইপ
ফাইল: index.html, style.css, app.js, manifest.json, sw.js, icon.svg

সীমাবদ্ধতা:
- এটি প্রথম UI প্রোটোটাইপ; সম্পূর্ণ প্রোডাকশন অ্যাপ নয়।
- Login ডেমো; তথ্য শুধু এই ব্রাউজারের localStorage-এ থাকে। প্রকৃত অ্যাকাউন্টের জন্য Supabase Auth ও নিরাপদ ডেটাবেস দরকার।
- পণ্য, দাম, টিকা, ভিডিও বর্তমানে নমুনা; অনলাইন Admin ও ডেটাবেস এখনও সংযুক্ত নয়।
- WhatsApp চালাতে app.js-এর CONFIG.whatsappNumber-এ নিজের নম্বর বসান। দেশ কোডসহ শুধু সংখ্যা দিন, যেমন 8801XXXXXXXXX-এ X বদলে নিজের নম্বর দিন।
- PWA ইনস্টল/অফলাইন ফিচারের জন্য HTTPS হোস্টিং দরকার। ফোনে শুধু index.html ফাইল খোলা পূর্ণ PWA নয়।
- টিকার সময়সূচি যাচাই করে তারপর প্রকাশ করবেন।

Android মোবাইল থেকে বিনামূল্যে হোস্টিং:
1) ZIP Extract করুন।
2) https://github.com/ এ ফ্রি অ্যাকাউন্ট খুলে New repository তৈরি করুন: khamaro-smart-farm (Public)।
3) Add file → Upload files থেকে সব ফাইল আপলোড করে Commit changes দিন।
4) Settings → Pages → Build and deployment-এ Deploy from a branch, branch main, folder /(root) নির্বাচন করে Save করুন।
5) Settings → Pages-এ তৈরি হওয়া URL Android Chrome-এ খুলুন।
6) Chrome-এর ⋮ → Add to Home screen / Install app চাপুন।

GitHub Pages শুধু static frontend হোস্ট করে; লগইন, অনলাইন Admin বা সার্ভার-ডেটাবেস দেয় না। সেগুলো পরের ধাপে Supabase দিয়ে যুক্ত করতে হবে।
