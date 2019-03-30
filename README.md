# Translation App

How to make translation app,tranlate language in android,How to change language in android?

#  Demo

Here is the link to download apk file
[Open APK File](https://github.com/kontashi35/Translation/blob/master/SimpleTranslation.apk).


#  Working

Here is the simple application which demonstrate how to make translation app.

#  Here is the heart code of application

1.  Helper class which is necessary for translation.copy and paste in new class call LocaleHelper.class

[Open LocaleHelper Class](https://github.com/kontashi35/Translation/blob/master/app/src/main/java/com/icthealth/translationapp/LocaleHelper.java
).


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
