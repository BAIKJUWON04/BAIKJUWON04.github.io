# BAIKJUWON04.github.io

백주원의 취업용 기술 블로그입니다.

- 주소: https://baikjuwon04.github.io
- GitHub: https://github.com/BAIKJUWON04
- 테마: Jekyll Chirpy

## 글 작성

`_templates`에서 원하는 템플릿을 복사한 후 `_posts`에 넣습니다.

파일 이름 형식:

```text
YYYY-MM-DD-title.md
```

예시:

```text
2026-08-18-esp32-uart.md
```

## 카테고리

글의 Front Matter에서 아래 다섯 카테고리 중 하나를 사용합니다.

```yaml
categories: [포트폴리오]
categories: [개발공부]
categories: [임베디드]
categories: [CS공부]
categories: [외부활동]
```

카테고리 기준 정보는 `_data/categories.yml`에서 관리합니다.

## 이미지

```text
assets/img/posts/
assets/img/projects/
```

Markdown 예시:

```markdown
![설명](/assets/img/posts/example.png)
```

## GitHub Pages 설정

GitHub 저장소의:

`Settings → Pages → Build and deployment → Source`

에서 **GitHub Actions**를 선택합니다.

그 뒤 `main` 브랜치에 반영하면 `.github/workflows/pages-deploy.yml`이 배포를 담당합니다.

## Velog 이전을 고려한 원칙

본문에는 일반 Markdown 문법을 우선 사용합니다.

- 제목
- 목록
- 표
- 코드 블록
- 이미지
- 링크

Jekyll 전용 Liquid 문법은 일반 글 본문에서는 가급적 사용하지 않습니다.
