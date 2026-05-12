# ✨ PetPals
반려동물 용품 쇼핑과 커뮤니티 기능을 결합한 이커머스 플랫폼입니다.
Django REST Framework와 React 기반으로 개발되었으며, 피드·팔로우·Q&A 등 SNS형 기능을 제공합니다.

---

## 📌 프로젝트 개요
PetPals는 반려동물 쇼핑 + 사용자 커뮤니티를 결합한 서비스를 목표로 합니다.
사용자는 상품을 탐색하고 구매할 뿐 아니라, 피드·후기·Q&A를 통해 실사용 정보를 얻을 수 있습니다.

### 🔎 기획 배경
- 반려동물 시장 확대 → 제품이 다양해지며 정보 분산  
- 실제 사용자 경험 기반 정보의 필요성 증가  
- 구매와 커뮤니티 흐름을 연결하는 서비스가 부족합니다.  

### 💡 해결 방향
- 피드 기반 SNS 기능 제공  
- 팔로우 구조로 네트워크·정보 순환 강화  
- 상품별 Q&A로 사용자 경험 공유  

---

## 🚀 핵심 기능

### 👤 사용자(User)
- 회원가입 / 로그인 
- 프로필 관리  
- 팔로우 / 언팔로우  
- 나의 피드 조회  

### 🛒 상품(Product)
- 카테고리별 상품 탐색  
- 옵션/재고 확인  
- 상품 상세 페이지  
- 장바구니 / 주문 / 결제  

### 📝 커뮤니티
- 피드 작성 / 수정 / 삭제  
- 팔로잉 기반 추천 피드  
- 제품별 Q&A (질문/답변)  

### 🛍 판매자(Seller)
- 판매자 인증  
- 상품 CRUD  
- **월별 매출 통계 대시보드 제공**

---

## 🛠 기술 스택

### Backend
- Python  
- Django / DRF  
- PostgreSQL  

### Frontend
- React  
- JavaScript  
- MUI  
- CKEditor  

### DevOps / Tools
- Docker / Docker-compose  
- GitHub Actions  
- Figma, Notion, draw.io  

---

## 🗂 데이터베이스 구조
총 **19개 테이블**로 구성된 ERD 기반 설계  
- User / Profile  
- Product / Category / Option / Inventory  
- Order / Payment  
- Feed / Comment / Follow  
- QnA / Answer  

(ERD 이미지는 `/docs/ERD.png` 형태로 추가 가능)

---

## 🔗 URL 설계 (일부)

| 기능 | URL | Method |
|------|------|--------|
| 회원가입 | `/users/register/` | POST |
| 로그인 | `/users/login/` | POST |
| 상품 목록 | `/products/` | GET |
| 상품 상세 | `/products/detail/{id}/` | GET |
| 주문 생성 | `/orders/create/` | POST |
| 피드 생성 | `/feed/create/` | POST |
| Q&A 상세 | `/board/qna/{id}` | GET |

---

## 👨‍💻 개인 기여도

### Backend Development
- User CRUD 및 JWT 인증 구현  
- Seller 인증 로직 개발  
- Product API 일부 설계 및 구조 정리  

### 📊 판매자 대시보드
- 월별 매출 Aggregation 로직 구현  
- 쿼리 최적화 및 데이터 구조 개선  

### ⚙️ 협업 효율화
- **GitHub Actions 기반 자동 코드 리뷰봇 구축**  
  - PR 기준 코드 검사  
  - 자동 리뷰 코멘트  
  - 팀 개발 속도 향상  

### 🎨 Frontend 협업
- 페이지 흐름(UI Flow) 개선  
- 피드·상품 화면 구성 일부 담당  

### 📚 문서화
- ERD 작성 일부 담당  
- API 명세 정리  
- 회의 운영 및 기능 정의 정리  

---

## 🔧 실행 방법

### Backend

```bash
git clone https://github.com/Hyeonboong/Petpals-Project.git
cd be
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

### Frontend

```bash
cd fe
npm install
npm run dev
```

---

## 🌟 프로젝트 의의
- 쇼핑과 커뮤니티 도메인의 결합을 직접 설계  
- 설계 → 개발 → 배포까지 전체 단계 경험  
- GitHub Actions 자동화로 효율적인 협업 경험  
- Django/React 기반 풀스택 프로젝트 경험 확보  
