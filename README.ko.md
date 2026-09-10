# XXD Panel 120｜건축 개념 손그림 기록

사진의 공간적 기억을 여백이 풍부한 건축 스케치로 만듭니다.

[简体中文](README.md) · [English](README.en.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [العربية](README.ar.md)

## 샘플 작품

本项目已发布 8 张实际样片，图片文件位于 `assets/examples/`。

| sample-05 | sample-06 |
| --- | --- |
| ![sample-05](assets/examples/sample-05.png) | ![sample-06](assets/examples/sample-06.png) |
| sample-07 | sample-08 |
| ![sample-07](assets/examples/sample-07.png) | ![sample-08](assets/examples/sample-08.png) |
| sample-09 | sample-10 |
| ![sample-09](assets/examples/sample-09.png) | ![sample-10](assets/examples/sample-10.png) |
| sample-11 | sample-12 |
| ![sample-11](assets/examples/sample-11.png) | ![sample-12](assets/examples/sample-12.png) |

## 적합한 상황과 해결하는 문제

사진 전체를 따라 그리지 않고 설계 탐색을 보여 주는 개념도가 필요할 때 적합합니다. Panel 120 은 정체성과 공간적 기억을 유지하면서 핵심 형태, 윤곽, 관계를 자유로운 투시 선화로 정제합니다. 소량의 색면, 기하학적 참조선, 넓은 여백이 작품을 구성합니다.

### 이런 상황에 적합합니다

- 건축, 공간, 여행, 사물 사진을 편집 감각의 개념 손그림으로 전환할 때.
- 약한 구도, 복잡한 배경, 작은 피사체를 삭제·재배치·크기 변화로 살릴 때.
- 전면 채색이나 사실적 완성도 없이 식별성과 공간 관계를 유지할 때.
- 대조 구성, 디자인 전용, 배경화면, 폴더 일괄 출력에 같은 스타일이 필요할 때.

### 해결하는 문제

- 배경과 부차적인 사물을 제거해 핵심 형태와 시각적 기억을 남깁니다.
- 절제되고 약간 반복되는 투시선과 구성선으로 설계 탐색을 표현합니다.
- 장식으로 화면을 채우지 않고 여백을 구도의 일부로 만듭니다.
- 대조 그림은 동일한 두 영역만 사용하며 원본별 독립 생성으로 이중 스타일 변환을 피합니다.

## 사용 팁

- **선명한 사진 한 장부터 시작하세요:** 피사체, 동작, 관계가 잘 보이는 이미지를 고른 뒤 출력 방식과 비율을 정합니다.
- **파라미터를 한 문장으로 연결하세요:** “상하 / 좌우 / 순수 디자인 + 16:9 / 3:4 / 휴대폰 배경화면”처럼 말하고 컴퓨터·태블릿·스마트워치 크기도 덧붙일 수 있습니다.
- **남겨야 할 것을 분명히 하세요:** 인물, 사물, 동작, 관계, 문구를 지정하되 레이아웃을 지나치게 고정하지 않아야 스타일이 자연스럽게 설계합니다.
- **텍스트 방식을 고르세요:** 이미지에서 지능적으로 생성하게 하거나, `--text exact --copy`로 정확한 문구를 고정하거나, `--text none`으로 글자를 없앨 수 있습니다.
- **사진 영역과 디자인 영역을 설명하세요:** 상하·좌우에서는 사진을 남길 쪽과 다시 디자인할 쪽을 말하고, 순수 디자인·배경화면은 전체 캔버스를 다시 설계한다고 알려 주세요.
- **한 장을 먼저 시험한 뒤 일괄 처리하세요:** 모드, 비율, 텍스트, 언어를 한 장에서 확인하고 같은 설정을 폴더에 적용합니다. 비교를 위해 한 번에 한 변수만 바꾸세요.

## 시작하기

```bash
git clone https://github.com/nevertoday/xxd-panel-120.git
npx skills add https://github.com/nevertoday/xxd-panel-120 --skill xxd-panel-120
```

설치 후 Agent 세션을 다시 시작하고 `$xxd-panel-120`을 호출하세요. 사용자 단위 Codex 설치에는 `--global --agent codex --yes`를 추가할 수 있습니다.

```text
/xxd-panel-120 photo.jpg --mode top-bottom --size 3:4 --text prompt --locale ko-KR
/xxd-panel-120 photo.jpg --mode left-right --size 16:9 --text prompt --locale en-US
/xxd-panel-120 photo.jpg --mode design-only --size 9:16 --text none
```

전체 실행 계약은 [SKILL.md](SKILL.md), 런타임 어댑터는 [영어](references/xxd-panel-120-prompt.en.md)와 [중국어](references/xxd-panel-120-prompt.zh-CN.md)를 확인하세요.

## 원본 프롬프트 · 5 개 언어

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

중국어 파일은 사용자 원문을 그대로 보존하며 실행 시 유일한 창작·미학 기준입니다. 다른 버전은 완전하고 충실한 읽기용 번역입니다.

건축 개념 투시 스케치 · 손 선화 · 기하학적 참조선 · 소량의 색과 그림자 · 원본에서 추출한 2–4 색 · 넓은 여백 · 최소 편집 주석

## 사진을 작품으로 만드는 과정

주제와 공간 관계 이해 → 핵심 형태 정제 → 복잡한 배경 삭제 → 크기와 자르기 재구성 → 투시선·기하학적 참조선·소량의 색면으로 재구축 → 여백과 짧은 주석으로 마무리

## 완성 작품의 특징

- 사진은 위 또는 왼쪽에 남고 미세한 색 보정만 하며 정체성과 자세를 유지합니다.
- 디자인은 건축 개념 손그림이며 전체 장면 복사, 사실적 완성도, 3D 가 아닙니다.
- 정제된 작은 피사체는 중심에서 벗어나거나 가장자리에 붙거나 일부 잘릴 수 있으며 여백이 구도에 참여합니다.
- 원본의 2–4 색으로 깨끗하고 절제된 색 체계를 만들고 핵심 부위에만 옅게 적용합니다.
- 기하학적 그림자는 부피와 깊이를 표현하고 소수의 보조선은 탐색의 느낌을 남깁니다.
- 소량의 글을 여백에 조용히 놓고 고정 글꼴 템플릿을 쓰지 않습니다. 샘플은 영어입니다。

선택한 출력 모드는 배치만 바꾸며 원문의 미적 요구는 유지합니다. `left-right` 는 위 사진을 왼쪽, 아래 디자인을 오른쪽으로 옮깁니다. 지정 비율은 원문의 기본 `3:4` 보다 우선합니다.

## 네 가지 출력 모드

- `top-bottom`: 전폭 상하 두 영역만 사용합니다. 실제 사진은 위, 디자인은 아래에 정확히 50%씩 둡니다.
- `left-right`: 전고 좌우 두 영역만 사용합니다. 실제 사진은 왼쪽, 디자인은 오른쪽에 정확히 50%씩 두며 상하 구도로 돌리지 않습니다.
- `design-only`: 전체 캔버스에 Panel 120의 디자인 번역만 표시하고 사진은 보이지 않는 참고 자료로 사용합니다.
- `wallpaper-pack`: 휴대폰, iPad, 데스크톱, 시계용 완성 이미지를 각각 만들며 `linked` 또는 `independent`를 선택합니다.

모드와 크기는 여러 개 선택할 수 있습니다. `1:1`, `3:4`, `4:3`, `4:5`, `5:4`, `2:3`, `3:2`, `9:16`, `16:9`, `21:9`, `5:7`, `7:5`, 정확한 픽셀을 지원합니다. 텍스트는 모델 생성, 사용자 원문, 없음 중에서 선택합니다. 폴더 입력은 각 소스를 분리 처리하고 최종 PNG를 하나의 새 작업 폴더에 평면으로 저장합니다.

<!-- xxd-readme-ads:start -->
## XXD 소개

XXD는 Xiaoxiaodong 브랜드 이름의 약자입니다. 이 프로젝트는 [@xiaoxiaodong01](https://x.com/xiaoxiaodong01)이 만들고 관리합니다.

## Xiaoxiaodong 멀티플랫폼 멤버십 · CNY 699/년

> **광고 안내:** 아래 QR 코드와 멤버십·유료 서비스 링크는 XXD의 홍보 정보입니다. 스캔이나 구매는 선택 사항이며 오픈 소스 이용에는 영향을 주지 않습니다.

연간 멤버십 하나로 **Knowledge Planet + XXD 회원 프롬프트 라이브러리 + 모든 General Skills 멤버십**을 함께 이용할 수 있습니다. 각각 따로 구매할 필요가 없습니다.

<!-- xxd-panel-command-system:start -->

### Skills가 함께 작동하는 방식

| 등급 | 포함 내용 | 역할 |
|---|---|---|
| **General** | [`xxd-panel-all`](https://github.com/xiaoxiaodong-ai/xxd-panel-all) | 사용 가능한 번호형 Skills를 찾고, 이미지·주제·용도에 맞춰 추천하며, 여러 스타일과 일괄 작업을 정리합니다. |
| **Soldier** | `xxd-panel-NNN` | 각 번호가 고유한 원본 프롬프트와 미학에 따라 General이 배정한 구체적인 작업을 완성합니다. |

<!-- xxd-panel-command-system:end -->

### 회원 혜택

1. **Xiaoxiaodong을 AI 학습 상담자로**
   [Knowledge Planet](https://wx.zsxq.com/group/15554814142882)에서 AI 학습, 도구, 실제 프로젝트에 대해 언제든 질문할 수 있습니다. 답변과 유용한 내용을 회원 자료로 계속 정리합니다.
2. **계속 업데이트되는 회원 프롬프트 라이브러리**
   [XXD 회원 프롬프트 라이브러리](https://vip.xiaoxiaodong.ai/)에는 현재 약 3만 2천 개의 프롬프트가 있으며, 10만 개 이상을 목표로 계속 확장합니다.
3. **모든 General Skills와 사용 지원**
   하나의 멤버십으로 모든 General Skills를 이용하고, 사용 중 도움이 필요할 때 안내와 Q&A를 받을 수 있습니다.
4. **필요성이 높은 요청을 우선 검토**
   회원이 제안한 수요가 높고 꼭 필요한 프롬프트와 Skills는 우선 검토하고 개발합니다.

### 가입 방법

- [회원 웹사이트에서 직접 가입](https://vip.xiaoxiaodong.ai/)할 수 있습니다.
- 또는 아래 QR 코드로 Xiaoxiaodong에게 연락하면 가입을 도와드립니다.

<p align="center"><a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="Xiaoxiaodong 연락처" width="280"></a></p>
<!-- xxd-readme-ads:end -->

## 라이선스

이 프로젝트(Skill, 프롬프트, 스크립트, 문서, 함께 제공되는 샘플 이미지 포함)는 **PolyForm Noncommercial License 1.0.0**을 따릅니다. 전체 법률 문구는 [LICENSE](LICENSE), 공식 페이지는 <https://polyformproject.org/licenses/noncommercial/1.0.0>에서 확인하세요.

쉽게 말하면 다음과 같습니다.

- 개인은 학습, 연구, 실험, 테스트, 취미 프로젝트, 사적 오락에 사용할 수 있습니다. 자선 단체, 교육 기관, 공공 연구·안전·보건 기관, 환경보호 단체, 정부 기관도 사용할 수 있습니다.
- **비상업적 목적**이라면 사용, 복사, 수정, 파생 작업 제작, 공유가 가능합니다. 공유할 때는 이 라이선스(또는 위 링크)와 저자가 제공한 모든 `Required Notice:` 문구를 함께 제공해야 합니다.
- 상업 제품이나 서비스, 유료 납품, 접근권 또는 라이선스 판매, 상업적 적용으로 이어질 것으로 예상되는 용도에는 사용할 수 없습니다. 상업적으로 사용하려면 저작권자에게 별도의 서면 허가를 받아야 합니다.
- 이 계약은 명시된 저작권 라이선스와 제한된 특허 라이선스만 부여합니다. 상표, 브랜드명 또는 명시되지 않은 다른 권리를 부여하지 않으며 라이선스를 제3자에게 재허여할 수도 없습니다.
- 서면으로 위반 통지를 받으면 32일 안에 준수 상태로 돌아가고 실질적인 시정 조치를 해야 하며, 그렇지 않으면 라이선스가 즉시 종료됩니다. 특허 침해를 서면으로 주장해도 특허 라이선스가 종료됩니다.
- 콘텐츠는 법이 허용하는 범위에서 어떠한 보증도 없이 “있는 그대로” 제공됩니다. 사용에 따른 위험과 잠재적 손실은 사용자가 부담합니다.
