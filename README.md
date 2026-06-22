KH정보교육원 Semi Project (2026.3.24 ~ 2026.4.22)

- 프로젝트 소개
중고 거래를 중심으로 커뮤니티 기능을 결합한 통합 서비스로, 이용자들이 중고 거래를 통해 자원 재사용을 실천하고 탄소 배출 감소에 기여할 수 있도록 돕는 프로젝트

- 주요 기능 및 기능 상세
(1) 회원가입 및 로그인
(2) 중고거래 게시판 및 관련 기능
(3) 커뮤니티 게시판 및 관련 기능
(4) 1:1 채팅 기능 (중고거래 게시판 한정)
(5) 내 정보 관련 및 포인트로 색상 변경
(6) 회원 등급 구분(슈퍼 관리자, 관리자, 일반 유저)
(7) 관리자 페이지 (회원 관리, 게시글 관리, 댓글 관리, 거래 현황)

포트폴리오 PPT 주소(공개 보기 링크 전용): https://canva.link/keghmh1725gz40x

Semi Project 원본 주소: https://github.com/lshlsh98/react_semi

Semi Project의 PPT 주소(공개 보기 링크 전용): https://canva.link/hwzg2pnrnn5bkbu

# ♻️ C2C (Customer To Carbon) - 중고거래 및 커뮤니티 사이트

팀 프로젝트

---

## 🛠 기술 스택

| 분류 | 기술 |
|------|------|
| **Frontend** | React 19, JSX, CSS Modules, Vite |
| **UI 라이브러리** | MUI (Material UI), Emotion |
| **에디터** | Tiptap (리치 텍스트 에디터) |
| **상태 관리** | Zustand |
| **HTTP 통신** | Axios |
| **실시간 통신** | WebSocket, STOMP, SockJS |
| **인증** | JWT (jwt-decode) |
| **알림** | SweetAlert2 (SWAL) |
| **차트** | Recharts |
| **주소 검색** | 카카오 우편번호 API |
| **Backend** | Spring Boot 4.0, Spring Security, Spring WebSocket |
| **ORM** | MyBatis |
| **Database** | Oracle |
| **인증** | JWT (jjwt) |
| **이메일** | Spring Mail |
| **기타** | Lombok, Jsoup |
| **버전 관리** | Git |

---

## 📋 기능 목록

| 페이지 | 세부 기능 | 기능 설명 | 로그인 여부 |
|--------|-----------|-----------|:-----------:|
| **회원** | 회원가입 | 이메일 인증 후 아이디·비밀번호·닉네임 입력하여 가입 | X |
| | 로그인 | 아이디·비밀번호 입력 후 JWT 토큰 발급 / 토큰 만료 시 자동 로그아웃 | X |
| | 아이디 찾기 | 이메일·닉네임 입력 시 아이디 조회 | X |
| | 비밀번호 찾기 | 이메일·아이디 일치 확인 후 임시 비밀번호 이메일 전송 | X |
| | 이메일 인증 | 6자리 랜덤 인증코드 이메일 발송 | X |
| **마이페이지** | 내 정보 수정 | 닉네임·비밀번호 변경, 프로필 썸네일 변경 | O |
| | 회원 탈퇴 | 회원 정보 및 프로필 이미지 삭제 | O |
| | 내 커뮤니티 게시글 | 내가 작성한 커뮤니티 글 목록 조회·숨김·삭제 | O |
| | 내 거래 게시글 | 내가 작성한 마켓 글 목록 조회·숨김·삭제 | O |
| | 내 댓글 관리 | 커뮤니티·마켓 댓글 목록 조회·수정·삭제 | O |
| | 좋아요·싫어요·신고 게시글 | 좋아요/싫어요/신고한 게시글 목록 조회 | O |
| | 거래 현황 차트 | Recharts로 거래 현황 시각화 | O |
| | 나의 인기글·최신글 | 내 인기글 및 최신글 조회 | O |
| | 색상 테마 변경 | 프로필 색상 테마 선택 및 변경 | O |
| **커뮤니티** | 게시글 목록 조회 | 필터·검색·페이지네이션 | X |
| | 게시글 등록 | Tiptap 에디터로 이미지 포함 글 작성 | O |
| | 게시글 상세 조회 | 게시글 단건 조회 (조회수 포함) | X |
| | 게시글 수정 | 본인 게시글 수정 | O |
| | 게시글 삭제 | 본인 게시글 삭제 | O |
| | 좋아요·싫어요 | 게시글 좋아요·싫어요 등록·취소 | O |
| | 게시글 신고 | 게시글 신고 등록·취소 | O |
| | 댓글·대댓글 CRUD | 댓글 및 대댓글 작성·수정·삭제 | O |
| | 댓글 좋아요·싫어요 | 댓글 좋아요·싫어요 등록·취소 | O |
| | 댓글 신고 | 댓글 신고 등록 | O |
| **중고거래 (마켓)** | 게시글 목록 조회 | 필터·검색·페이지네이션 | X |
| | 게시글 등록 | 이미지 포함 거래 글 작성 | O |
| | 게시글 상세 조회 | 게시글 단건 조회 (조회수 포함) | X |
| | 게시글 수정 | 본인 게시글 수정 (이미지 추가·삭제) | O |
| | 게시글 삭제 | 본인 게시글 삭제 (이미지 함께 삭제) | O |
| | 좋아요 | 게시글 좋아요 등록·취소 | O |
| | 게시글 신고 | 게시글 신고 등록·취소 | O |
| | 거래 요청 | 거래 요청 등록·조회·취소 | O |
| | 거래 확정 | 거래 확정 처리 | O |
| | 댓글·대댓글 CRUD | 댓글 및 대댓글 작성·수정·삭제 | O |
| | 댓글 신고 | 댓글 신고 등록 | O |
| | 탄소 기여도 | 회원별 탄소 기여도 목록 조회 | X |
| **채팅** | 실시간 채팅 | WebSocket + STOMP 기반 1:1 실시간 채팅 | O |
| | 채팅방 생성·조회 | 마켓 게시글 기준 채팅방 개설 또는 기존 방 반환 | O |
| | 채팅 내역 조회 | 이전 채팅 메시지 목록 조회 | O |
| | 메시지 읽음 처리 | 채팅 메시지 읽음 상태 처리 | O |
| | 내 채팅방 목록 | 참여 중인 채팅방 목록 조회 | O |
| | 거래 완료 시 채팅방 삭제 | 거래 확정 시 해당 채팅방 자동 삭제 | O |
| **지도** | 지도 조회 | 카카오 지도 API 기반 지역 검색 | X |
| **메인 페이지** | 커뮤니티 인기글·최신글 | 메인용 커뮤니티 게시글 목록 조회 | X |
| | 마켓 최신 목록 | 메인용 마켓 게시글 목록 조회 | X |

---

## 📡 API 명세

### 👤 회원 (Member)

| Method | URL | 설명 | 인증 필요 |
|--------|-----|------|:---------:|
| POST | /members | 회원가입 | X |
| GET | /members/exists?memberId= | 아이디 중복 확인 | X |
| POST | /members/email-verification | 이메일 인증번호 발송 | X |
| POST | /members/login | 로그인 (JWT 발급) | X |
| POST | /members/find-id | 아이디 찾기 | X |
| POST | /members/find-pw | 비밀번호 찾기 (임시 비밀번호 이메일 전송) | X |
| GET | /members/{memberId} | 회원 정보 조회 | X |
| GET | /members | 전체 회원 목록 조회 | X |
| POST | /members/pw-auth | 비밀번호 인증 | O |
| PATCH | /members/{memberId}/thumbnail/update | 프로필 썸네일 변경 | O |
| PATCH | /members/{memberId} | 회원 정보 수정 | O |
| PATCH | /members/update-pw | 비밀번호 변경 | O |
| DELETE | /members/{memberId} | 회원 탈퇴 | O |

### 🏠 마이페이지 (Mypage)

| Method | URL | 설명 | 인증 필요 |
|--------|-----|------|:---------:|
| GET | /mypages/board/community | 내 커뮤니티 게시글 목록 조회 | O |
| PATCH | /mypages/board/community/{boardNo} | 커뮤니티 게시글 숨김 처리 | O |
| DELETE | /mypages/board/community/{boardNo} | 커뮤니티 게시글 삭제 | O |
| GET | /mypages/board/market | 내 마켓 게시글 목록 조회 | O |
| PATCH | /mypages/board/market/{boardNo} | 마켓 게시글 숨김 처리 | O |
| DELETE | /mypages/board/market/{boardNo} | 마켓 게시글 삭제 | O |
| GET | /mypages/comment/market | 내 마켓 댓글 목록 조회 | O |
| GET | /mypages/comment/community | 내 커뮤니티 댓글 목록 조회 | O |
| PATCH | /mypages/comment/{commentNo} | 댓글 수정 | O |
| DELETE | /mypages/comment/{commentNo} | 댓글 삭제 | O |
| GET | /mypages/board/likedislike | 좋아요·싫어요·신고 게시글 목록 조회 | O |
| GET | /mypages/tradestatus/chart | 거래 현황 차트 데이터 조회 | O |
| GET | /mypages/tradestatus/list | 거래 현황 목록 조회 | O |
| GET | /mypages/today/{memberId} | 오늘의 활동 통계 조회 | O |
| GET | /mypages/my-best/{memberId} | 내 인기글 조회 | O |
| GET | /mypages/my-recent/{memberId} | 내 최신글 조회 | O |
| GET | /mypages/color | 색상 테마 목록 조회 | O |
| PATCH | /mypages/color | 색상 테마 변경 | O |
| GET | /mypages/report/{boardNo} | 신고 목록 조회 | O |
| GET | /mypages/report/private/{boardNo} | 내 신고 조회 | O |

### 📝 커뮤니티 (Community)

| Method | URL | 설명 | 인증 필요 |
|--------|-----|------|:---------:|
| GET | /communities | 게시글 목록 조회 | X |
| GET | /communities/main?type= | 메인 페이지용 게시글 목록 조회 | X |
| POST | /communities | 게시글 등록 | O |
| GET | /communities/{communityNo} | 게시글 상세 조회 | X |
| PUT | /communities/{communityNo} | 게시글 수정 | O |
| DELETE | /communities/{communityNo} | 게시글 삭제 | O |
| PATCH | /communities/view/{communityNo} | 조회수 증가 | X |
| GET | /communities/{communityNo}/likes | 좋아요 정보 조회 | X |
| POST | /communities/{communityNo}/likes | 좋아요 등록 | O |
| DELETE | /communities/{communityNo}/likes | 좋아요 취소 | O |
| GET | /communities/{communityNo}/dislikes | 싫어요 정보 조회 | X |
| POST | /communities/{communityNo}/dislikes | 싫어요 등록 | O |
| DELETE | /communities/{communityNo}/dislikes | 싫어요 취소 | O |
| GET | /communities/{communityNo}/reports | 신고 정보 조회 | X |
| POST | /communities/{communityNo}/reports | 신고 등록 | O |
| DELETE | /communities/{communityNo}/reports | 신고 취소 | O |
| GET | /communities/{communityNo}/comments | 댓글 목록 조회 | X |
| POST | /communities/comments | 댓글·대댓글 등록 | O |
| PATCH | /communities/comments | 댓글 수정 | O |
| DELETE | /communities/comments/{communityCommentNo} | 댓글 삭제 | O |
| GET | /communities/comments/{communityCommentNo}/likes | 댓글 좋아요 정보 조회 | X |
| POST | /communities/comments/{communityCommentNo}/likes | 댓글 좋아요 등록 | O |
| DELETE | /communities/comments/{communityCommentNo}/likes | 댓글 좋아요 취소 | O |
| POST | /communities/comments/{communityCommentNo}/dislikes | 댓글 싫어요 등록 | O |
| DELETE | /communities/comments/{communityCommentNo}/dislikes | 댓글 싫어요 취소 | O |
| POST | /communities/comments/reports | 댓글 신고 | O |

### 🛒 중고거래 (Market)

| Method | URL | 설명 | 인증 필요 |
|--------|-----|------|:---------:|
| GET | /markets | 게시글 목록 조회 | X |
| GET | /markets/main | 메인 페이지용 게시글 목록 조회 | X |
| POST | /markets | 게시글 등록 (이미지 포함) | O |
| GET | /markets/{marketNo} | 게시글 상세 조회 | X |
| PUT | /markets/{marketNo} | 게시글 수정 | O |
| DELETE | /markets/{marketNo} | 게시글 삭제 (이미지 함께 삭제) | O |
| POST | /markets/{marketNo}/likes | 좋아요 등록 | O |
| DELETE | /markets/{marketNo}/likes | 좋아요 취소 | O |
| POST | /markets/{marketNo}/reports | 신고 등록 | O |
| DELETE | /markets/{marketNo}/reports | 신고 취소 | O |
| POST | /markets/{marketNo}/request | 거래 요청 등록 | O |
| GET | /markets/{marketNo}/requests | 거래 요청 목록 조회 | O |
| PATCH | /markets/{marketNo}/requests/{buyerId} | 거래 확정 | O |
| DELETE | /markets/{marketNo}/request | 거래 요청 취소 | O |
| GET | /markets/{marketNo}/comments | 댓글 목록 조회 | X |
| POST | /markets/comments | 댓글·대댓글 등록 | O |
| PATCH | /markets/comments | 댓글 수정 | O |
| DELETE | /markets/comments/{commentNo} | 댓글 삭제 | O |
| POST | /markets/comments/reports | 댓글 신고 | O |
| GET | /markets/carbon-contribution/{memberId} | 탄소 기여도 조회 | X |

### 💬 채팅 (Chat)

| Method | URL | 설명 | 인증 필요 |
|--------|-----|------|:---------:|
| GET | /chat/history/{roomId} | 이전 채팅 메시지 조회 | O |
| POST | /chat/room/{roomId}/read | 메시지 읽음 처리 | O |
| GET | /chat/my/rooms | 내 채팅방 목록 조회 | O |
| POST | /chat/room/private/create | 1:1 채팅방 생성 또는 기존 방 반환 | O |
| DELETE | /chat/room/private/{marketNo} | 거래 완료 시 채팅방 삭제 | O |
| STOMP | /publish/{roomId} | 실시간 메시지 전송 | O |
| STOMP | /topic/{roomId} | 실시간 메시지 수신 (구독) | O |

