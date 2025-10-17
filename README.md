# EntropyLab — GitHub Pages Template

엔트로피 혼합(빨강/파랑 입자)과 온도차(평균 속도 차)를 시각화하는 **정적 웹 시뮬레이터** 템플릿입니다.  
단일 `index.html`만으로 동작하며, GitHub Pages에 바로 배포할 수 있습니다.

## 파일 구성
```
.
├─ index.html              # 인터랙티브 시뮬레이터 (순수 HTML/CSS/JS)
├─ favicon.svg             # 파비콘
├─ LICENSE                 # MIT 라이선스
├─ .gitignore
└─ .github/
   └─ workflows/
      └─ pages.yml         # (선택) Actions로 GitHub Pages 배포
```

## 빠른 시작
1. 새 GitHub 리포지토리를 만들고(공개 권장) 이 파일들을 업로드합니다.
2. **방법 A — Settings 사용(가장 간단)**  
   - Repo → **Settings → Pages** → *Build and deployment*에서  
     **Source: Deploy from a branch**, **Branch: `main` (root)** 선택 → **Save**.  
   - 잠시 후 표시되는 URL로 접속합니다.
3. **방법 B — GitHub Actions 사용**  
   - 이 템플릿의 `.github/workflows/pages.yml`을 그대로 사용합니다.  
   - Repo → **Settings → Pages** → *Source: GitHub Actions* 로 설정합니다.

## 사용 팁
- 좌우 구획은 중앙 막으로 나뉘며, 막을 열면 입자가 섞입니다.
- 엔트로피 표시는 좌/우 점유 비율 `p` 기반의 **정규화된 Shannon 혼합 엔트로피**입니다.
- 열 흐름을 간단히 표현하기 위해 왼쪽 평균 속도 스케일(ΔT)을 조절할 수 있습니다.
- 스냅샷 버튼으로 PNG 이미지를 다운로드할 수 있습니다.

## 확장 아이디어
- Clausius 정의 \(dS = \delta Q/T\)를 반영하려면, 격자 온도장과 입자-격자 간 에너지 교환(속도 재샘플링) 모델을 추가하세요.
- 격자를 더 세분화하여 \(H = -\sum_i p_i \log p_i\) 형태의 공간 분포 엔트로피로 확장할 수 있습니다.
- i18n(영/한) 토글, 다크/라이트 테마 스위치, 모바일 UI 최적화 등.

## 라이선스
MIT — 자유롭게 수정/배포하세요. 크레딧으로 이 리포를 링크해주시면 큰 도움이 됩니다 🙌