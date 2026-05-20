# MkDocs 시작하기

## 소개

이 문서는 MkDocs를 처음 사용할 때 필요한 기본 흐름을 간단히 정리한 가이드입니다.

MkDocs는 Markdown 파일을 기반으로 정적 문서 사이트를 만들어주는 도구입니다. Material 테마를 함께 사용하면 검색, 다크 모드, 코드 복사 버튼, 네비게이션 탭 등 문서 사이트에 필요한 기능을 쉽게 추가할 수 있습니다.

## 목차

- [MkDocs란?](#mkdocs란)
- [기본 설치](#기본-설치)
- [프로젝트 생성](#프로젝트-생성)
- [로컬 서버 실행](#로컬-서버-실행)
- [문서 작성 흐름](#문서-작성-흐름)

## MkDocs란?

MkDocs는 Markdown으로 작성한 문서를 HTML 사이트로 변환해주는 정적 사이트 생성기입니다.

기술 문서, 개발 노트, 프로젝트 가이드, API 문서 등을 정리할 때 유용합니다.

## 기본 설치

Python이 설치되어 있다면 다음 명령어로 MkDocs와 Material 테마를 설치할 수 있습니다.

```bash
pip install mkdocs mkdocs-material
```

설치가 완료되었는지 확인하려면 다음 명령어를 실행합니다.

```bash
mkdocs --version
```

## 프로젝트 생성

새 MkDocs 프로젝트는 다음 명령어로 만들 수 있습니다.

```bash
mkdocs new my-tech-notes
cd my-tech-notes
```

기본 구조는 보통 다음과 같습니다.

```text
my-tech-notes/
├─ docs/
│  └─ index.md
└─ mkdocs.yml
```

## 로컬 서버 실행

문서를 작성하면서 결과를 바로 확인하려면 다음 명령어를 사용합니다.

```bash
mkdocs serve
```

실행 후 브라우저에서 아래 주소로 접속하면 문서 사이트를 확인할 수 있습니다.

```text
http://127.0.0.1:8000
```

## 문서 작성 흐름

MkDocs 문서 작성의 기본 흐름은 다음과 같습니다.

1. `docs` 폴더 안에 Markdown 파일을 작성합니다.
2. `mkdocs.yml` 파일에서 사이트 이름, 테마, 메뉴 구조를 설정합니다.
3. `mkdocs serve`로 로컬에서 확인합니다.
4. 문서가 완성되면 GitHub Pages 등으로 배포합니다.

처음에는 복잡하게 시작하기보다, 자주 보는 명령어와 오류 해결 방법부터 하나씩 정리하는 것이 좋습니다.
