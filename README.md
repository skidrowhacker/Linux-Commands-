# Linux-Commands - By Skidrow | Yasser [ Twitter @firfox20 ] 

[ Linux ]  - [ File Commands  - اوامر ادارة الملفات] 
#
ls  [Directory Listing ] [ ااستعرض مجلد ] 
ls - al [ Listing Directory with Hidden Files] [ استعرض المجلد والملفات المخفية ]
cd  [Change directory] [ للتغيير الى مسار اخر ] 
pwd  [to print current directory/ path]  [ لطباعة المسار الحالي ] 
mkdir  [to make directory ][ لانشاء مجلد ] 
rm   [to delete file [ لحذف ملف ] 
rm - r [to delete file with ask to delete each time] [ لحذف ملف مع اظهار رسالة بتاكيد الحذف ] 
rm - rf [to forcly delete the file without prior premssions] [ لحذف الملف بجميع محتوياته بدون اي تاكيد ] 
cp file1 [ to copy file1] [  [ لنسخ ملف 1]
cp -r dir [to copy directory[ [ لنسخ مجلد ]
mv file1 [ to rename / move file1 ] [ لنقل او اعادة تسمية ملف1]
touch file.txt [ to create file.txt]  - [ لانشاء ملف ] 
cat file.txt [ to see the contents of a file ] - [ لعرض محتوى ملف ] 
more file.txt [ to see the contents of a file ] - [ لعرض محتوى ملف ] 
head file.txt [ to see first 10 lines of a file] - [ لعرض اول 10 اسطر من الملف ]
tail file.txt [ to see last 10 lines of a file ] - [لعرض اخر 10 اسطر من الملف ] 
tail -f file.txt [ to monitor the file of any changes added ] [ لمراقبة اي اضافات تطري على الملف ] 
sudo sed -i '/wordhere/d' filepath [ to remove specif word from a file [لازالة كلمة معينة من ملف ما ]
wc    [ to check for wordcount / how many  ]  [ لمعرفة عدد الاسطر او عدد ملفات بمسار ما ] 
grep kali /etc/passwd [ to search for word kali in the specifed file ] [ للبحث عن كلمة كالي بالمسار المعطى ] 
find /etc/passwd  [ to search for the given file name ] [ للبحث عن الملف المعطى بمجلدات النظام ]
echo 'hello' > file.txt  [ to print hello to a file.txt] [ لطباعة مرحبا في ملف ]
echo 'hello2' >> file.txt [ to add word  hello2  to the same file.txt ]
#
[Linux ] - [ Systeminfo  - تفاصيل النظام] 
date  [show the current date & time] [ لعرض التاريخ والوقت الحالي ] 
cal  [to show the calander of the month] - [ لعرض التقويم للشهر الحالي ] 
uptime [ to show current system uptime ] - [ لعرض مدة الجهاز وهو يعمل ]
w  [to show current user online] - [ لعرض الحساب المتصل ] 
whoami  [to show the current user logged into]  [ لعرض الحساب المسجل دخول به انت حاليا ] 
finger kali - [to show info about user kali] [ لعرض معلومات عن اليوزر كالي ]
uname -a [to show the OS & Kernal info] - [ لعرض تفاصيل كاملة عن نظام التشغيل والاصدار واصدار الكيرنل ]
cat /proc/cpuinfo  [ to show info about cpu ] -  [ لعرض معلومات عن المعالج ] 
cat /proc/meminfo [ to show info about memory ] -  [ لعرض معلومات عن الذاكرة ] 
man    [ to show os & tools Manual ] - [ عرض كتيب تفاصيل او طريقة الاستخدام للنظام والادوات ]
df   [ th show Disk Usage ] - [ عرض تفاصيل استهلاك الاقراص ] 
du   [ show directoy space usage ] - [ لعرض استهلاك مساحة المسارات ] 
free [ show memory and swap usage ]  - [ لعرض تفاصيل عن استهلاك الذاكرة والبارتيشن ] 
whereis [ location of app ]  - [ للبحث عن ملف او مسار  تطبيق ] 
which  [show  locate the executable file associated with the given command  ]  - [ لعرض مسار التنفيذ لاداة او تطبيق ما ] 
#
[Linux ] - Compression [ ضغط وفك ضغط ملفات ]
tar cfz file.tgz file -P   [to Tar Files] - [ لضغط الملفات ] 
tar xfv file.tgz  [to untar files  ] - [ لفك ضغط الملفات ] 
gzip -d file.tar.gz  [ in case of .gz  uncompress] - [ في حالة الملف .gz فك ضغط ] 
#
[Linux ]  - [P0roess Managment] =  [ ادارة عمليات النظام ] 
ps  [ display active process  ]  - [ لعرض العمليات الحالية]
top [ display all running process [ لعرض جميع العمليات الحالية ] 
kill 120 [ to kill processs with number 120 ] [ لاغلاق العملية رقم 120 من التشغيل ] 
killall apache2 [ to kill all process named apache2 ] - [ لاغلاق جميع العمليات اللي تحمل اسم اباشتي 2 ]
bg  [ list stopped / working in background  porcess ] - [ لعرض العمليات المتوقفة او اللي تعمل بالخلفية ] 
fg  [ list bring background process to main or resume suspended one ] - [ لاحضار عملية بالخلفية الى اساسية او اعادة تشغيل عملية متوقفة ]
#
[Linux ] - [Network ]  - [ اوامر شبكات ] 
ping google.com [ to ping host google.com and see its alive or not ]  - [ ارسال حزم لفحص موقع قوقل هل يستجيب ام لا ] 
whois google.com [ to check details about google web ] - لمعرفة تفاصيل عن الموقع قوقل ]
dig google.com [to check for dns info ] - [ لمعرفة تفاصيل الدي ان اس الخاص بقوقل ] 
dig -x google.com [ reverse loookup host ] [ للبحث العكسي عن الموقع قوقل ]
wget file [ to get file ] = [ لتحميل او احضار ملف ] 
wget -c file [ to resume the download of a file ] - [ لاستكمال عملية التنزيل لملف ما ] 
ifconfig - [to show your network interfaces] = [ لمعرفة تفاصيل محولات الشبكة الخاصة بك ] 
iwconfig [ to show wifi network interfaces ] - [ لعرض محولات الشبكة الاسلكية ] 
traceroute google.com - [ to send packets from router to wbesite and check its recived or not ] [ لاختبار عملية الارسال والتتبع من الرواتر للموقع] 
netstat [ Print network connections, routing tables ] - [ لطباعة تفاصيل اتصالات الشبكة والتوجيه] 
ss  [ show more tcp coneections on network sockests ] - [ لعرض تفاصيل عن اتصالات الشبكة وبروتوكلات التي سي بي ] 
route [ route - show / manipulate the IP routing table] - [ لعرض او تعديل التوجيهات الخاصة بالشبكة ] 
host google.com [ DNS lookup utility ] - [ اداة بحث عن تفاصيل الدي ان اس للموقع وطباعة الايبياهات]
hostname  [display the system's DNS name] - [لطباعة الدي ان اس الخاص بالنظام او التعديل عليه ] 
curl [ transfering data from / to ]  [ اداة تستعمل في نقل من والى ] 
ifplugstatus [ link beat detection tool ] - [ لاختبار اللينكات المتصلة بالجهاز]
iftop  [ display network bandwith usage , network monitor connections ] - [ لفحص الاتصالات والاستهلاك الخاص بالشبكة ] 
tcpdump [ dump traffice of network ]  - [ لمعرفة تفاصيل اتصالات الشبكة والحزم ] 
#
[Linux] - [File / Premessions ] - [ /الصلاحيات/ الملفات والمجلدات ]
chmod [ to change file premssion [ لتغيير صلاحية مجلد/ملف ما ]
chmod +x [ to give execute premssions ] [ لاعطاء صلاحية تنفيذ ]
chmod +rw [ to giv read & write premssions ] - [ لاعطاء صلاحية قراءة وكتابة ] 
chmod -R [ to give premssions to main file and all other files ] [ لاعطاء صلاحية للملف الاساسي وجميع الملفات الاضافية ]
chown kali /home/Desktop/ [ to set owner ship of file / directory ] - [ لتعديل ملكية ملف او مجلد او مسار ما ]
chown -R kali /home/Desktop/ [ to set owner ship of file / directory with all sub files  ] - [  لتعديل ملكية ملف او مجلد او مسار ما والملفات الاضافية معه  ]
getent group |grep kali [ to check to which group kali is added to ] - [ لمعرفة الى اي مجموعات في النظام مضاف عليها اليوزر كالي ]
useradd -c 'Skidrow account' -m skidrow  [to add a user account to linux ]   [ لاضافة حساب جديد الى النظام باسم سكدرو ]
userdel -r skidrow - to remove  [to remove user from the account ] - [ لازالة الحساب سكدرو من النظام ] 
usermod -aG sudo username [ add a user to group sudo [ لاضافة مستخدم الى مجموعة سودو ]
gpasswd -d whoami sudo  [ remove user from group sudo ] - [لازالة المستخدم من مجموعة سودو ]
sudo su  [ to login with root privleges user ] [ لتسجيل الدخول بيوزر روت صلاحيات عليا ] 
#












#
Refrancess to Linux Commands [ افضل المراجع لتعلم بقية الاوامر ] 
https://www.javatpoint.com/linux-commands
https://www.geeksforgeeks.org/linux-commands/
http://111000.net/systems/files/The_Linux_Command_Line-arabic-14.07.pdf
