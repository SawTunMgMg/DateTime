# DateTime
JSON projects များမှာ date နဲ့ time အတွက်ကို "timestamp" = "1357000" ဆိုပီး ဂဏန်းများနဲ့ ပေးထားရင် ဒီ DateTime.java လေးကို သုံးနိုင်ပါတယ်
အသုံးပြုနည်းများ
------------

၁။ လက်ရှိ ရက်စွဲ အချိန်ရဲ့ မီလီစက္ကန့် long တန်ဖိုး ရယူနည်း
-------------------


DateTime.getNow();

၂။ မီလီစက္ကန့် long တန်ဖိုးကို ရက်စွဲ String ပြောင်းယူခြင်း
-------------------

DateTime.Date(long Ticks);


ဥပမာ ဒီနေ့ရဲ့ ရက်စွဲ String လိုချင်ရင်
-------------------

String today=DateTime.Date(DateTime.getNow());

"01/08/2017" ရပါမယ်။ ရက်/လ/နှစ် ပုံစံနဲ့ ဖြစ်ပါတယ်။ ဒီပုံစံကို စိတ်ကြိုက် ပြောင်းနိုင်တယ်။


၃။ မီလီစက္ကန့် long တန်ဖိုးကို အချိန် String ပြောင်းယူခြင်း
-------------------

DateTime.Time(long Ticks);

ဥပမာ လက်ရှိ ရက်စွဲ အချိန် ရဲ့ အချိန် String လိုချင်ရင်

String time=DateTime.Time(DateTime.getNow());

"11:20:25" ရပါမယ်။ နာရီ/မိနစ်/စက္ကန့် ပုံစံနဲ့ ဖြစ်ပါတယ်။ ဒီပုံစံကို စိတ်ကြိုက် ပြောင်းနိုင်တယ်။


၄။ ရက်စွဲ String တခုကို မီလီစက္ကန့် long တန်ဖိုးအဖြစ် ပြောင်းယူခြင်း
-------------------

DateTime.DateParse(String date);

ဥပမာ

long birthday= DateTime.DateParse("01/01/1990");


၅။ အချိန် String တခုကို မီလီစက္ကန့် long တန်ဖိုးအဖြစ် ပြောင်းယူခြင်း
-------------------

DateTime.TimeParse(String time);

ဥပမာ

long birthtime= DateTime.TimeParse("01:45:40");


၆။ ရက်စွဲ String နဲ့ အချိန် String ကနေ မီလီစက္ကန့် long တန်ဖိုးအဖြစ် ပြောင်းယူခြင်း
-------------------

DateTime.DateTimeParse(String Date, String Time)

ဥပမာ

long birth_day_time= DateTime.DateTimeParse("01/01/1990","01:45:40");


၇။ TimeZone သတ်မှတ်ခြင်း
-------------------

DateTime.SetTimeZone(int OffsetHours);


၈။ မီလီစက္ကန့် long တန်ဖိုးကနေ ခုနှစ် သက္ကရာဇ် ရယူခြင်း (int)
-------------------

DateTime.GetYear(long Ticks);

ဥပမာ လက်ရှိ အချိန်ရဲ့ ခုနှစ် လိုချင်ရင်

int year=DateTime.GetYear( DateTime.getNow());


၉။ မီလီစက္ကန့် long တန်ဖိုးကနေ လ ဂဏန်း ရယူခြင်း (int)
-------------------

DateTime.GetMonth(long Ticks);

ဥပမာ လက်ရှိ အချိန်ရဲ့ လ လိုချင်ရင်

int month=DateTime.GetMonth( DateTime.getNow());


၁၀။ မီလီစက္ကန့် long တန်ဖိုးကနေ ရက် ဂဏန်း ရယူခြင်း (int)
-------------------

DateTime.GetDayOfMonth(long Ticks);

ဥပမာ လက်ရှိ အချိန်ရဲ့ ရက် လိုချင်ရင်

int dayOfMonth=DateTime.GetDayOfMonth( DateTime.getNow());


၁၁။ မီလီစက္ကန့် long တန်ဖိုးကနေ နှစ်အစက ရေတွက်တဲ့ ရက် ဂဏန်း ရယူခြင်း (int)
-------------------

DateTime.GetDayOfYear(long Ticks);

ဥပမာ လက်ရှိ အချိန်ရဲ့၊ နှစ်အစက ရေတွက်တဲ့ ရက် လိုချင်ရင်

int dayOfYear=DateTime.GetDayOfYear( DateTime.getNow());


၁၂။ မီလီစက္ကန့် long တန်ဖိုးကနေ နေ့ ဂဏန်း ရယူခြင်း (int)။ တနင်္ဂနွေ =1 စသည်။
-------------------

DateTime.GetDayOfWeek(long Ticks);

ဥပမာ လက်ရှိ အချိန်ရဲ့ နေ့ လိုချင်ရင်

int day=DateTime.GetDayOfWeek( DateTime.getNow());


၁၃။ မီလီစက္ကန့် long တန်ဖိုးကနေ နာရီ ဂဏန်း ရယူခြင်း (int)
-------------------

DateTime.GetHour(long Ticks);

ဥပမာ လက်ရှိ အချိန်ရဲ့ နာရီ လိုချင်ရင်

int hour=DateTime.GetHour( DateTime.getNow());


၁၄။ မီလီစက္ကန့် long တန်ဖိုးကနေ မိနစ် ဂဏန်း ရယူခြင်း (int)
-------------------

DateTime.GetMinute(long Ticks);

ဥပမာ လက်ရှိ အချိန်ရဲ့ မိနစ် လိုချင်ရင်

int minute=DateTime.GetMinute( DateTime.getNow());


၁၅။ မီလီစက္ကန့် long တန်ဖိုးကနေ စက္ကန့် ဂဏန်း ရယူခြင်း (int)
-------------------

DateTime.GetSecond(long Ticks);

ဥပမာ လက်ရှိ အချိန်ရဲ့ စက္ကန့် လိုချင်ရင်

int second=DateTime.GetSecond( DateTime.getNow());


၁၆။ မီလီစက္ကန့် long တန်ဖိုးတခုသို့ နှစ်၊ လ၊ ရက် တန်ဖိုး ပေါင်းထည့်ခြင်း (long)
-------------------

DateTime.Add(long Ticks, int Years, int Months, int Days)

ဥပမာ မွေးနေ့ ကနေ ၁၀ နှစ်၊ ၆ လ၊ ၁၂ ရက် အကြာမှာ ရှိတဲ့ ရက်စွဲ String ရှာကြည့်ပါမယ်။

String birthday="12/10/1990";
long birth=DateTime.DateParse(birthday);
long newDateMilli=DateTime.Add(birth,10,6,12);

String newDate=DateTime.Date( newDateMilli);

