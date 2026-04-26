1. Important Commands

pwd
ls
ls -la
cd
mkdir
cp
mv
rm
cat
head -n
tail -n
grep
printf
wc
echo
source
export
cut
2. Git Commands

git init
git add .
git commit -m "..."
git log --oneline
./scripts/report.sh
3. Result Executing Command

git log --oneline
4. Short Assessment Questions
ما الفرق بين > و >> و &> ؟
> : يعيد توجيه المخرجات القياسية (stdout) إلى ملف مع الكتابة فوق المحتوى (overwrite).
>> : يعيد توجيه المخرجات القياسية إلى ملف مع الإضافة في نهاية المحتوى (append).
&> : يعيد توجيه المخرجات القياسية + رسائل الخطأ (stdout + stderr) إلى ملف.
متى نستخدم source بدل ./script.sh ؟
نستخدم source script.sh لتشغيل السكريبت داخل نفس الـ shell، وبالتالي تبقى المتغيرات والدوال بعد التنفيذ.
بينما ./script.sh يشغّل السكريبت في subshell، وبالتالي لا تبقى المتغيرات بعد انتهاء التنفيذ.
ما الفرق بين && و || ؟
&& : ينفذ الأمر الثاني فقط إذا نجح الأول.
|| : ينفذ الأمر الثاني فقط إذا فشل الأول.
لماذا نستخدم الفروع (Branches) في Git؟
للفصل بين التطوير والنسخة المستقرة.
لتجربة ميزات جديدة بدون التأثير على المشروع الأساسي.
لتسهيل العمل الجماعي ومراجعة التعديلات.
ما وظيفة ssh-agent؟
إدارة مفاتيح SSH الخاصة بالمستخدم.
تخزين بيانات الدخول مؤقتًا لتجنب إدخال كلمة المرور في كل مرة عند الاتصال بالخوادم.
