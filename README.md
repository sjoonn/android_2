# <div align="center">로또 번호 뽑기</div>

# <div align="center">👋🏻 처음 화면 👋🏻</div>
### TextView(제목)와 CheckBox, 그리고 아래에 버튼 3개가 보인다.
![스크린샷 2022-08-17 오전 11 20 22](https://user-images.githubusercontent.com/102125786/185020849-3406c4f8-81b5-42f9-af75-6df273b817cd.png)

# <div align="center">📱 사용 방법 📱</div>
## <div align="center"> 중복 허용 체크박스 X </div>
### 로또 번호 생성 하기 버튼을 누른다. 무작위로 중복 되지 않은 6가지의 로또번호가 나온다.
![스크린샷 2022-08-17 오전 11 30 43](https://user-images.githubusercontent.com/102125786/185021578-ab36b3f1-3d67-4986-8e5e-fe1693773ee1.png)

### 그리고 나온 숫자를 저장하기 버튼으로 저장한다.
![스크린샷 2022-08-17 오전 11 32 45](https://user-images.githubusercontent.com/102125786/185021808-1edc272b-c68d-467e-b847-dbb3044bbc2f.png)

### 이 과정을 여러번 반복후 버튼을 눌러 리스트로 볼 수 있다.(최대 30번)
![스크린샷 2022-08-17 오전 11 39 25](https://user-images.githubusercontent.com/102125786/185022536-1a3142e1-7b58-492b-bfb4-d745c66066c9.png)

### 저장한 내용은 다시 저장 할수없다.
![스크린샷 2022-08-17 오전 11 46 38](https://user-images.githubusercontent.com/102125786/185023634-989dee8e-89b3-4758-9ae6-3e941d2fd605.png)

### 30번 저장한후 또 저장하기를 누르면 저장공간 부족이 뜬다.
![스크린샷 2022-08-17 오전 11 42 52](https://user-images.githubusercontent.com/102125786/185023029-7596b2c7-b88f-476a-b04a-8e9067e996ab.png)

## <div align="center"> 중복 허용 체크박스 O </div>
### 중복 허용을 하면 중복된 숫자도 나온다.
![스크린샷 2022-08-17 오전 11 52 15](https://user-images.githubusercontent.com/102125786/185024100-193f65b2-d330-4465-906d-1e66f52db544.png)

## <div align="center"> 😅 고치지 못한 오류 😅 </div>
### 중복 허용을 누르면 마지막 숫자가 모두 0으로 나온다.
![스크린샷 2022-08-17 오전 11 52 15](https://user-images.githubusercontent.com/102125786/185024166-4285a971-b690-446c-8790-b97a306cafc4.png)

# <div align="center"> ✍🏻 중요한 내용 ✍🏻 </div>
### 로또 공(drawble)
```kotlin
   <?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android"
    android:shape="oval">
    <solid android:color="#0000ff"/>
    <size
        android:width="50dp"
        android:height="50dp"/>>
</shape>
```

### binding(build.gradle)
```kotlin
   buildFeatures{
        viewBinding true
    }
```

### binding(MainActivity)
```kotlin
   private lateinit var binding: ActivityMainBinding
   override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        binding = ActivityMainBinding.inflate(layoutInflater)
        setContentView(binding.root)
```

### 
