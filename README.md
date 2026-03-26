# MUST — Project Page

Project page for **"MUST: Modality-Specific Representation-Aware Transformer for Diffusion-Enhanced Survival Prediction with Missing Modality"** (CVPR 2026).

🔗 **Live page**: [https://kylekwkim.github.io/MUST-official/](https://kylekwkim.github.io/MUST-official/)

---

## Setup & Deployment (Step-by-Step)

### Step 1. GitHub 레포지토리 생성

1. [GitHub](https://github.com)에 로그인
2. 우측 상단 `+` → **New repository** 클릭
3. Repository name: `MUST-official`
4. Public으로 설정
5. **Create repository** 클릭

### Step 2. 파일 업로드

#### 방법 A — GitHub 웹에서 직접 업로드
1. 새로 만든 레포지토리 페이지에서 **"uploading an existing file"** 클릭
2. 이 폴더의 모든 파일을 드래그 & 드롭:
   - `index.html`
   - `static/images/Figure_main.png` (논문의 main figure)
3. **Commit changes** 클릭

#### 방법 B — Git CLI 사용
```bash
git clone https://github.com/KyleKWKim/MUST-official.git
cd MUST-official

# 이 폴더의 파일들을 복사
cp /path/to/index.html .
mkdir -p static/images
cp /path/to/Figure_main.png static/images/

git add .
git commit -m "Add project page"
git push origin main
```

### Step 3. Figure 이미지 추가

`static/images/` 폴더에 논문의 메인 figure를 `Figure_main.png`로 넣어주세요.

### Step 4. GitHub Pages 활성화

1. 레포지토리 → **Settings** 탭
2. 좌측 메뉴 **Pages** (Code and automation 섹션 아래)
3. **Source** 드롭다운: `Deploy from a branch` 선택
4. **Branch**: `main`, 폴더: `/ (root)` 선택
5. **Save** 클릭

약 1~2분 후 `https://kylekwkim.github.io/MUST-official/` 에서 페이지가 활성화됩니다.

### Step 5. 링크 업데이트 (추후)

`index.html`에서 아래 항목들을 업데이트하세요:

| 항목 | 현재 상태 | 업데이트 방법 |
|------|-----------|---------------|
| Paper PDF | `disabled` | `class="link-btn"` + `href="PDF_URL"` |
| arXiv | `disabled` | `class="link-btn"` + `href="https://arxiv.org/abs/XXXX.XXXXX"` |
| Code | `disabled` | `class="link-btn"` + `href="https://github.com/KyleKWKim/MUST-official"` |
| Video | `disabled` | `class="link-btn"` + `href="VIDEO_URL"` |

예시 — arXiv 링크 활성화:
```html
<!-- Before -->
<a class="link-btn disabled" href="#" title="Coming Soon">

<!-- After -->
<a class="link-btn" href="https://arxiv.org/abs/XXXX.XXXXX" target="_blank">
```

---

## 파일 구조

```
MUST-official/
├── index.html              # 메인 프로젝트 페이지
├── static/
│   └── images/
│       └── Figure_main.png # 논문 메인 figure
└── README.md               # 이 파일
```

## Citation

```bibtex
@inproceedings{kim2026must,
  title     = {MUST: Modality-Specific Representation-Aware
               Transformer for Diffusion-Enhanced Survival
               Prediction with Missing Modality},
  author    = {Kim, Kyungwon and Hwang, Dosik},
  booktitle = {Proceedings of the IEEE/CVF Conference on
               Computer Vision and Pattern Recognition (CVPR)},
  year      = {2026}
}
```

## Acknowledgements

This work was supported by the National Research Foundation of Korea (NRF) grant funded by the Korea government (MSIT) (No. RS-2025-16070382, RS-2025-02215070, RS-2025-02217919), Artificial Intelligence Graduate School Program at Yonsei University (RS-2020-II201361), the Korea Institute of Science and Technology (KIST) Institutional Program under Grant 26E0170.

Project page template inspired by [Nerfies](https://nerfies.github.io).
