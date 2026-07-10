# Ninja Survival Unity Archive

이 저장소는 `닌자 서바이벌`의 기존 Unity 구현물을 보존하기 위한 아카이브 저장소다.

## 목적

- Unity에서 어느 정도 구현된 원본 프로젝트를 안전하게 보존한다.
- Godot/GDScript 재구현 작업에서 참고할 수 있도록 기존 시스템, 애셋, 씬, 스크립트를 남긴다.
- 앞으로 실제 개발 기준은 별도 Godot 저장소 `ninja-survival-godot`에서 진행한다.

## 현재 상태

Unity ZIP 업로드가 확인되었다.

- 확인 커밋: `99c241a979649b1f0a7574c2d39e11ca73e67cdc`
- 파일명: `ninza.zip`

현재 ChatGPT/GitHub 커넥터에서는 ZIP 바이너리 내부를 직접 풀어 분석할 수 없었다. 다음 단계는 Codex 또는 로컬 환경에서 ZIP을 풀고 `Assets/`, `Packages/`, `ProjectSettings/` 구조를 확인하는 것이다.

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
