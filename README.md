# Translation App
How to make translation app,tranlate language in android
#  Working
Here is the simple application which demonstrate how to make translation app.
#  Here is the heart code of application
1.  Helper class which is necessary for translation.copy and paste in new class call LocaleHelper.class

https://github.com/kontashi35/Translation/blob/master/app/src/main/java/com/icthealth/translationapp/LocaleHelper.java

2.  override your language changing activity like this.

      ```  @Override
        protected void attachBaseContext(Context base) {
        super.attachBaseContext(LocaleHelper.onAttach(base));
        }
        ```
3.  When you change in language call this function.

       ``` private void updateViews(String languageCode) {
        Context context = LocaleHelper.setLocale(this, languageCode);
        Resources resources = context.getResources();
        

        }
        ```
    4.That it.Enjoy!!!
