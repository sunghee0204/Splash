# Splash

<a>https://kagus2.tistory.com/24</a>


```
AUTHORIZATION_FAILED: invalid android_key_hash or ios_bundle_id or web_site_url
-> openssl로 키 해쉬 생성 시 문제가 된 것
안드로이드의 경우 안드로이드 스튜디오의 플랫폼 폴더가 아니라 프로젝트의 android 폴더 아래에 있는 키를 참조하여 생성해야 한다.
```

## kotlin version probelm (build.gradle)
/android/build.gradle
```
ext{ kotlinVersion = '1.5.31' }
dependencies { classpath("org.jetbrains.kotlin:kotlin-gradle-plugin:$kotlinVersion") }
```

## Execution failed for task ':app:packageDebug'
<a>https://hwangtaehyun.github.io/blog/android_emulator/OutOfMemory_Error/</a>

/android/app/src/main/AndroidManifest.xml
```
<applicaiton>
android:largeHeap=”true”
/>
```
