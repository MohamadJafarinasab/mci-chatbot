ابتدا از سایت https://alphacephei.com/vosk/models یک مدل سبک برای زبان فارسی دانلود کردم به نام vosk-model-small-fa-0.4 و آن را در درایو شخصی قرار دادم.

در محیط google colab مدل را unzip کردم.

با دستور pip3 install vosk آماده ی استفاده از vosk شدم.

همان طور که راهنمایی کرده بودید از کد https://github.com/alphacep/vosk-api/blob/master/python/example/test_simple.py استفاده کردم با دو تغییر.

به جای wf = wave.open(sys.argv[1], "rb") آرگومان ورودی را اسم فایل صوتی گذاشتم برای مثال wf = wave.open("/content/Weather.wav", "rb").

محتوای این فایل جمله ی "امروز هوا خیلی خوبه" است.

به جای model = Model(lang="en-us") از model = Model(model_name="vosk-model-small-fa-0.4") استفاده کردم.

تصویر نتیجه ی نهایی را مشاهده نمایید.




![task-001](https://user-images.githubusercontent.com/113296484/189542361-bb6465dc-72f1-48ea-8194-e2e76c0111a2.png)
