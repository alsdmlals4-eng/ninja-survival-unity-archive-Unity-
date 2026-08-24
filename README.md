# Ninja Survival Unity Archive

이 저장소는 `닌자 서바이벌`의 기존 Unity 구현물을 보존하기 위한 아카이브 저장소다.

## 목적

- Unity에서 어느 정도 구현된 원본 프로젝트를 안전하게 보존한다.
- Godot/GDScript 재구현 작업에서 참고할 수 있도록 기존 시스템, 애셋, 씬, 스크립트를 남긴다.
- 앞으로 실제 개발 기준은 별도 Godot 저장소 `ninja-survival-godot`에서 진행한다.

## 현재 상태

Unity ZIP 업로드 및 아카이브 인벤토리 확인이 완료되었다. 이 저장소는 **ARCHIVE_ONLY**이며 실제 제품 정본이나 구현 대상으로 사용하지 않는다.

- 감사 기준 커밋: `a6499f0e62175609147bd2d66b6c48b16cb2331e`
- 파일명: `ninza.zip`
- SHA-256: `72e08c6d552ea5dfd25175082844cf360dd40eb3bf53544f229aae2887f20491`
- 인벤토리/증거 한계: [`ARCHIVE_MANIFEST.md`](ARCHIVE_MANIFEST.md)

2026-08-24 감사에서 ZIP 중앙 디렉터리로 `Assets/`, `Packages/`, `ProjectSettings/` 루트를 확인했다. 이것은 파일 보존/검사 가능성만 뜻하며 Unity import/build/run, 시각·사운드 품질, 플레이 가능성, 기기 검증, 자산 권리를 뜻하지 않는다. 해당 상태는 모두 `NOT_RUN`이다.

## 권장 업로드 방식

Unity 프로젝트 전체를 올릴 때는 아래 폴더와 파일을 보존한다.

```text
Assets/
Packages/
ProjectSettings/
```

아래 폴더는 GitHub에 올리지 않는다.

```text
Library/
Temp/
Obj/
Build/
Builds/
Logs/
UserSettings/
.vs/
```

ZIP 스냅샷 보존이 목적이라면 ZIP 파일도 허용한다. 단, 이후 Codex가 분석하려면 ZIP을 풀어 실제 Unity 폴더 구조를 확인해야 한다.

## Godot 전환 원칙

Unity 코드는 Godot 코드로 직접 번역하지 않는다. Unity 구현은 참고 자료로만 사용하고, Godot 버전은 Godot 4.x + GDScript + Scene/Node 구조에 맞춰 재설계한다.

전환 대상 저장소:

```text
https://github.com/alsdmlals4-eng/ninja-survival-godot
```
