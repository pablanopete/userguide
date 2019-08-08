<!-- [![Documentation Status](https://readthedocs.org/projects/polkadot-wiki/badge/?version=latest)](https://polkadot-wiki.readthedocs.io/en/latest/?badge=latest)
[![CircleCI](https://circleci.com/gh/w3f/polkadot-wiki.svg?style=svg)](https://circleci.com/gh/w3f/polkadot-wiki) -->

# 쿠사마 사용자 설명서

이 리포지토리는 [쿠사마 사용자 설명서](https://guide.kusama.network)를 위한 리소스 파일을 담고 있습니다.

## 로컬 환경에서 실행하기

파이썬과 함께 설치되는 `pip` 패키지 매니저가 필요합니다.

자신의 컴퓨터에 리포지토리를 클론해주세요.

```bash
git clone https://github.com/kusamanetwork/userguide.git
```

 by using 
`pip` 패키지 매니저를 통해 `mkdocs`를 설치해주세요

```bash
pip install mkdocs --user
```

다시 `pip`를 통해 필요한 패키지들을 다운로드 받으세요.

```bash
pip install -r requirements.txt
```

`mkdocs serve` 명령어를 프로젝트 루트 디렉토리에서 실행하여 핫 리로딩되는 개발 서버를 구축한 뒤 웹 브라우져에서 `localhost:8000`주소에 연결하세요.

## 퍼블리싱

위키는 [문서 읽기](https://readthedocs.org)링크에 호스팅 되며 깃허브 리포지토리의 master 브랜치로 오는 커밋들로 만들어집니다.

## 스타일링

[Mkdocs-Material](https://squidfunk.github.io/mkdocs-material/)이 본 웹사이트의 테마를 만드는데 쓰였습니다.

## 컨트리뷰팅

[CONTRIBUTING](CONTRIBUTING.md) 문서 안에 있는 규칙들을 읽어보시기 바랍니다.

### 컨트리뷰터 전용 셋업

내용 편집 외 컨트리뷰터로 프로젝트를 셋업하려면, 로컬 환경에 클론된 리포지토리에서 `npm i` 커맨드를 실행해야 합니다.

### 새 페이지 더하기

새 페이지를 더하고자 한다면 새 페이지에 대한 링크를 따로`mkdocs.yml`에서 명시하여`nav` 필드를 수정해주세요. 이렇게 함으로서 한 주제에 관련하여 더 정갈하게 배치를 할 수 있거니와 페이지를 보여주는 방법도 깔끔해집니다.

### 맞춤법 검사

저희는 [`husky`](https://github.com/typicode/husky) 를 이용하여 택스트들의맞춤법을 검사합니다. 만약 커밋을 하는게 막혀져 있다면 `npm run spellcheck:interactive` 명령을 실행하여 인터랙티브 디버거를 실행한 뒤 맞춤법을 고치세요.
