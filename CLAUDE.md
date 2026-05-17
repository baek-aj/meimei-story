# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 프로젝트 개요

**우리는 메이메이 입니다** — 2005년 일산은혜교회 목장에서 시작된 공동체의 이야기를 기록하는 정적 블로그.

- **기술 스택**: Jekyll + Chirpy 테마, GitHub Pages 호스팅
- **배포**: `main` 브랜치에 push하면 GitHub Actions가 자동 빌드 및 배포
- **블로그 URL**: `https://baek-aj.github.io/meimei-story`

## 포스트 작성

새 포스트는 `_posts/` 디렉토리에 `YYYY-MM-DD-제목.md` 형식으로 생성:

```markdown
---
title: "모임 제목"
date: YYYY-MM-DD
categories: [모임]
tags: [연도, 장소]
image:
  path: /assets/images/YYYY-MM/대표사진.jpg
  alt: 사진 설명
---

내용
```

- **카테고리**: `모임`, `이야기`, `역사` 중 선택
- **날짜는 과거도 가능**: 파일명의 날짜로 정렬 — 2005년 이야기도 `2005-01-01-...md`로 소급 등록 가능
- 사진은 `assets/images/YYYY-MM/` 폴더에 저장

## 로컬 미리보기 (선택 사항)

```bash
bundle install
bundle exec jekyll serve
# → http://localhost:4000/meimei-story
```

Ruby 3.x + Bundler 필요. 연 2~3회 업데이트이므로 GitHub 웹 에디터로 직접 작성해도 무방.

## 설정 변경

`_config.yml`에서 블로그 기본 정보 수정. 변경 후 main 브랜치에 push하면 자동 반영.
