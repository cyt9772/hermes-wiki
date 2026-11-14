---
title: The Quick Python Book
created: 2026-11-14
updated: 2026-11-14
type: entity
tags: [book, programming, python, reference]
sources: [raw/books/quick-python-book.md]
confidence: medium
---

# The Quick Python Book

> 'a guide to learning and effectively using the Python language' — 핵심 기능부터 고급 주제로 이어지는 Python 개요+참고서 (표지·back cover)
## 개요
- **Author:** Daryl Harms, Kenneth McDonald (p3)
- **Publisher:** Manning Publications Co. (Greenwich, CT, p4) | **Pages:** 437
- **Positioning:** Python 핵심 기능(구문, 제어 흐름, 기본 자료구조)을 빠르게 익히고 객체지향·고급 문자열 처리 등으로 확장하는 실용 서적으로, 언어 창시자 Guido van Rossum이 특별 장을 집필 (back cover, p437).
## 내용
- 구성: Part I Starting (About Python / About the book / Getting started) → Part II The essentials (The Quick Python overview, absolute basics, lists/tuples, strings, dictionaries, control flow, functions, modules, file system, files, exceptions, scripts, classes/OOP, GUI/Tk) (p5-6).
- 고급/특수 주제: Tkinter 기반 GUI, MS Windows COM, CGI/Web, HTML 생성, Java 스크립팅 등 'What's inside' 항목으로 정리 (p437).
- C 확장 모듈: `PyArg_ParseTuple`로 인자 해석, `Py_BuildValue`로 반환값 구성, `PyMethodDef` 목록과 `Py_InitModule` 초기화 함수까지 C에서 Python 모듈을 작성하는 템플릿 제시 (p275).
- 메모리 관리: Python에서는 참조 카운트 기반 가비지 컬렉션이 allocation/de-allocation을 담당하므로 개발자가 직접 관리할 필요가 없음을 설명, Guido van Rossum의 *Extending and Embedding the Python Interpreter*를 참고문헌으로 제시 (p275).
- 평가: Fredrik Lundh 'concise overview with a compact reference' 등 전문가 서문(endorsement)이 뒷표지에 수록 (p437).
## 관련 페이지
- [[linear-algebra-for-programmers]] — 프로그래머 대상 기초/자료구조 학습 계열
- [[matlab-intro-and-use-kim]] — 데이터 분석 언어 입문서와 비교
