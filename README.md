# android-techlabs-library Maven Repository

이 리포는 [thyadang-techlabs/android-techlabs-library](https://github.com/thyadang-techlabs/android-techlabs-library)의 빌드 산출물을 보관하는 Maven 저장소야.

**직접 수정 금지** — 모든 파일은 소스 리포의 GitHub Actions가 자동으로 publish한다.

사용 가능한 버전 목록은 [`com/techlabs/android-techlabs-library/`](./com/techlabs/android-techlabs-library/) 디렉토리를 참조해.

---

## 설치

### 1. 사용 측 `settings.gradle.kts`에 Maven 저장소 추가

```kotlin
dependencyResolutionManagement {
    repositories {
        google()
        mavenCentral()
        maven {
            url = uri("https://raw.githubusercontent.com/thyadang-techlabs/android-techlabs-library-release/main/")
        }
    }
}
```

### 2. 앱 `build.gradle.kts`에 의존성 추가

```kotlin
dependencies {
    implementation("com.techlabs:android-techlabs-library:1.0.3")
}
```

---

이 README는 소스 리포의 `release-repo-README.md`에서 옮겨온 템플릿. 수정 시 소스 리포 쪽도 함께 갱신.
