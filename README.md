# GIT CHEAT SHEET

### টুল কনফিগার
#### লোকাল রিপোজিটরির জন্য টুল কনফিগার করা
###### নাম ঠিক করুন যেটা আপনি কমিট ট্রান্সেকশনের সাথে সংযুক্ত করতে চান।
```
$ git config --global user.name "[name]"
```
###### ইমেইল ঠিক করুন 
```
$ git config --global user.email "[email address]"
```

### রিপোজিটরি তৈরি
#### নতুন রিপোসিটোরি শুরু অথবা একটি বিদ্যমান URL থেকে শুরু করুন।
###### নির্দিষ্ট নাম দিয়ে একটি নতুন রিপোসিটোরি তৈরি করুন।
```
$ git init [project-name]
```
###### একটি repository এবং তার সম্পূর্ণ সংস্করণ ইতিহাস ডাউনলোড করুন।
```
$ git clone [url]
``` 


### পরিবর্তন করা
#### সম্পাদনা পর্যালোচনা করুন এবং একটি কমিট ট্রান্সেকসন ক্রাফট করুন।
###### সকল ফাইল লিস্ট করুন যা কমিট করা হবে।
```
$ git status
```
###### ফাইলগুলোর পার্থক্য দেখুন যেগুলো এখনো staged হয়নি।
```
$ git diff
```
###### সংস্করনের জন্য প্রস্তুতি ফাইল স্ন্যাপশট করুন।
```
$ git add [file]
```
###### staging এবং last file version এরমধ্যে পার্থক্য দেখুন।
```
$ git diff --staged
```
###### ফাইল Unstages, কিন্তু তার বিষয়বস্তু অপরিবর্তিত রাখুন।
```
$ git reset [file]
```
###### ফাইলের স্ন্যাপশট ভার্শনের ইতিহাসে সংরক্ষন করুন।
```
$ git commit -m"[descriptive message]"
```


### গ্রুপ পরিবর্তন
###### বর্তমান রিপোসিটোরির মধ্যে সব লোকাল ব্রাঞ্চ তালিকাভুক্ত করুন।
```
$ git branch
```
###### একটি নতুন ব্রাঞ্চ তৈরি করুন
```
$ git branch [branch-name]
```
###### নির্দিষ্ট শাখায় সুইচ এবং আপডেট ওয়ার্কিং ডিরেক্টরি
```
$ git checkout [branch-name]
```
###### বর্তমান শাখায় নির্দিষ্ট শাখার ইতিহাস একত্রিত করুন
```
$ git merge [branch-name]
```
###### নির্দিষ্ট শাখা মুছে ফেলে
```
$ git branch -d [branch-name]
```


### সিঙ্ক্রোনাইজড পরিবর্তনগুলি
#### একটি দূরবর্তী (URL) নিবন্ধন করুন এবং রিপোসিটোরি ইতিহাস এক্সচেঞ্জ করুন
###### দূরবর্তী রিপোসিটোরি থেকে সব ইতিহাস ডাউনলোড করুন
```
$ git fetch [remote]
```
###### বর্তমান স্থানীয় শাখা ও দূরবর্তী শাখা একত্রিত করুন
```
$ git merge [remote]/[branch]
```
###### সকল লোকাল ব্রাঞ্চ কমিট গিটহাবে আপলোড করুন
```
$ git push [remote] [branch]
```
###### বুকমার্ক হিস্টোরি ও অন্তর্ভুক্ত পরিবর্তনগুলো ডাউনলোড করুন
```
$ git pull
```


*(UNDER CONSTRUCTION)*
