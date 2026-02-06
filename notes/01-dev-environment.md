# 01. 개발 환경 설정

## 핵심 정리

### .NET SDK 확인
```bash
dotnet --version    # 설치된 버전 확인
```

### 프로젝트 생성 & 실행
```bash
dotnet new console -n 프로젝트이름    # 콘솔 프로젝트 생성
dotnet run                            # 빌드 + 실행
dotnet build                          # 빌드만
dotnet new list                       # 템플릿 목록 보기
```

### 프로젝트 구조
```
프로젝트이름/
├── 프로젝트이름.csproj    ← 프로젝트 설정 파일 (빌드 타겟, 패키지 등)
├── Program.cs             ← 메인 코드 파일
├── bin/                   ← 빌드 결과물
└── obj/                   ← 빌드 임시 파일
```

### .csproj 파일 구조
```xml
<Project Sdk="Microsoft.NET.Sdk">
  <PropertyGroup>
    <OutputType>Exe</OutputType>              <!-- 실행 파일 -->
    <TargetFramework>net10.0</TargetFramework> <!-- .NET 버전 -->
    <ImplicitUsings>enable</ImplicitUsings>    <!-- 기본 using 자동 포함 -->
    <Nullable>enable</Nullable>                <!-- null 안전성 체크 -->
  </PropertyGroup>
</Project>
```

### 최상위 문 (Top-level Statements)
- C# 9부터 지원
- `Main` 메서드 없이 바로 코드 작성 가능
- 내부적으로는 `Main` 메서드 구조가 그대로 존재

```csharp
// 최상위 문 (현재 방식)
Console.WriteLine("Hello, World!");

// 예전 방식 (C# 9 이전)
using System;
namespace HelloCSharp
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello, World!");
        }
    }
}
```

## 사용 도구
- VS Code
- .NET 10.0 SDK
