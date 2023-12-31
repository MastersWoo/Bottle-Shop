![1  Bottle Shop_Mainjpg](https://github.com/MastersWoo/Bottle-Shop/assets/123873604/4c83681d-869d-4465-9af4-bfebdfcad452)

프로젝트 기간: 2023.02.13 - 2023.02.03 

# 프로젝트 소개

세계적인 와인들을 즐길 수 있는 와인 쇼핑몰 Bottleshop

와인과 함께 곁들일 수 있는 여러 종류의 치즈도 판매하는 온라인 와인 쇼핑몰을 만들고자 했습니다.

배포 주소 : http://34.64.96.43/categories

# 서비스 주요 기능

<details>
<summary>사용자 관련 기능</summary>
<div markdown="1"> 
      
    ● 회원가입 - 회원가입 폼의 입력 값이 조건에 안 맞을 시 (이메일 형식, 비밀번호와 비밀번호확인의 일치 여부 등) 이를 사용자에게 알려준다.
      
    ● 회원가입 - 조건에 맞게 입력 후 제출 버튼을 누를 시, 백엔드 서버와 연결되어 회원가입 정보가 db에 저장된다.
    
    ● 로그인 - 로그인 폼의 입력 값이 조건에 안 맞을 시 (이메일 형식이 안 맞거나, 비밀번호가 틀리거나 등) 이를 사용자에게 알려준다.
    
    ● 로그인 - db에 저장된 정보로 로그인 성공 시, JWT 토큰이 프론트 단(sessionStorage, localStorage 등)에 저장되고, 다른 페이지(랜딩페이지, 상품페이지 등)로 이동한다.
    
    ● 로그아웃 - 로그아웃 시, 프론트 단에 저장되어 있던 JWT토큰이 제거된다.
    
    ● 사용자 정보 조회 - 사용자는 개인 페이지에서 자신의 회원 정보를 조회할 수 있다.
    
    ● 사용자 정보 수정 -  사용자는 개인 페이지에서 자신의 회원 정보를 수정할 수 있다.
    
    ● 사용자 정보 삭제 -  사용자는 개인 페이지에서 자신의 회원 정보를 삭제(탈퇴)할 수 있다.
    
    ● 관리자 기능 - 관리자 계정이 존재하며, 일반 사용자 계정과 구분된다.
    
    ● 사용자 정보 - db에 사용자의 이메일, 이름, 비밀번호(해쉬화된 문자열), 주소를 저장할 수 있다.

</div>
</details>

<details>
<summary>상품(제품) 관련 기능</summary>
<div markdown="1"> 
      
    ● 카테고리 조회 - 사용자가 카테고리 목록을 화면에서 확인할 수 있다.
    
    ● 카테고리 추가 - 관리자는 관리자 페이지에서, 상품이 속할 카테고리를 추가할 수 있다.
    
    ● 카테고리 수정 - 관리자는 관리자 페이지에서, 상품이 속할 카테고리 관련 데이터 (카테고리 이름 등)를 수정할 수 있다.
    
    ● 카테고리 삭제 - 관리자는 관리자 페이지에서, 상품이 속할 카테고리 관련 데이터를 삭제할 수 있다.
    
    ● 상품 추가 - 관리자는 관리자 페이지에서 상품을 추가할 수 있다.
    
    ● 상품 수정 - 관리자는 관리자 페이지에서 상품 관련 데이터를 수정할 수 있다.
    
    ● 상품 삭제 - 관리자는 관리자 페이지에서 상품 관련 데이터를 삭제할 수 있다.
    
    ● 상품 정보 - 상품은 특정 카테고리에 속해 있다.
    
    ● 상품 목록 - 사용자가 특정 카테고리를 선택할 시, 해당 카테고리에 속한 상품 목록이 화면에 나타난다.
    
    ● 상품 상세 - 사용자가 특정 상품을 선택할 시, 해당 상품의 상세 정보가 화면에 나타난다.
    
    ● 상품 정보 - db에 상품의 이름, 가격, 설명, 제조사를 저장할 수 있다.

</div>
</details>

<details>
<summary>장바구니 관련 기능</summary>
<div markdown="1">

    ● 장바구니 관련 데이터는 백엔드 데이터베이스가 아닌, 프론트단(localStorage, sessionStorage, indexedDB 등)에서 관리된다.
    
    ● 프론트 단에, 장바구니에 속한 상품 관련 데이터가 저장되어서, 페이지를 새로고침해도 장바구니에 상품들이 그대로 남아 있다.
    
    ● 장바구니 추가 - 사용자는 상품을 장바구니에 추가할 수 있다.
    
    ● 장바구니 수정 - 사용자는 장바구니에 속한 상품의 수량을 수정할 수 있다.
    
    ● 장바구니 전체 삭제 - 사용자는 장바구니에서, 버튼 1번의 클릭으로, 장바구니 상의 전체 상품을 제거할 수 있다.
    
    ● 장바구니 부분 삭제 - 사용자는 장바구니에서, 일부 상품을 골라서 제거할 수 있다.
    
    ● 장바구니 조회 - 사용자는 장바구니에 담긴 상품 목록을 확인할 수 있다.
    
    ● 장바구니 가격 조회 - 사용자는 장바구니에 담긴 상품들의 총 가격을 확인할 수 있다.

</div>
</details>

<details>
<summary>주문 관련 기능</summary>
<div markdown="1">

    ● 주문 추가 - 사용자는 장바구니에 속한 상품들로 주문을 추가(진행)할 수 있다.
    
    ● 주문 수정 - 관리자는 사용자의 주문 내역에서 배송 상태를 수정할 수 있다.
    
    ● 주문 수정 - 사용자는 주문 완료 후 배송이 시작되기 전까지 주문 정보를 수정할 수 있다.
    
    ● 주문 완료 - 주문 완료 시, 주문 완료 페이지로 이동한다.
    
    ● 주문 조회 - 사용자는 개인 페이지에서 자신의 주문 내역을 조회할 수 있다.
    
    ● 주문 조회 - 관리자는 관리 페이지에서 사용자들의 주문 내역을 조회할 수 있다.
    
    ● 주문 취소 - 사용자는 개인 페이지에서 자신의 주문 내역을 취소할 수 있다.
    
    ● 주문 삭제 - 관리자는 관리 페이지에서 사용자들의 주문 내역을 삭제할 수 있다.
    
    ● 주문 정보 - db에 배송 상태가 저장된다.
    
    ● 주문 정보 - db에 배송지 정보, 주문 총액, 수령자 이름 및 연락처가 저장된다.

</div>
</details>

## 프로젝트 구성도

● Tools: Tech

   □ 프론트엔드

    - Javascript, React, Bootstrap

   □ 백엔드

    - Node.js, Express.js, MongoDB

● 화면 흐름도 (Flow chart)

![image](https://github.com/MastersWoo/Bottle-Shop/assets/123873604/d07161f5-25f6-4829-86c9-934622c3b74d)

● Branch Strategy

| Branch Name   | 설명                       |
|---------------|--------------------------|
| dev           | 개발 브랜치                   |
| feature_front | 프론트 기능 구현 후 1차 merge 브랜치 |
| feature_back  | 백앤드 기능 구현 후 1차 merge 브랜치 |

 ● Commit Convention      
| 태그 이름 | 설명 |
| --- | --- |
| [FEAT] | 새로운 기능 구현 |
| [CHORE] | 코드 수정 및 추가, 기능 구현중 |
| [ADD] | 라이브러리 추가, 새로운 파일 생성 |
| [DEL] | 쓰지 않는 코드 삭제 |
| [FIX] | 버그 수정, 오류 해결 |
| [MOVE] | 프로젝트 내 파일이나 코드의 이동 |
| [RENAME] | 파일 이름 변경 |
| [DOCS] | README, WIKI 등 문서 개정 |
| [REFACTOR] | 코드 전면 수정이 있을 때 |
| [HOTFIX] | 급한 버그 수정 (issue, QA) |
| [MERGE] | 원격, 로컬 저장소에서 Merge 할 때 사용 |
| [RESOLVE] | confilct 고쳤을 때 |

● Codding Convention
 <details>
 <summary>변수명</summary>
 <div markdown="1"> 
      
 - 변수명은 항상 Carmel Case 사용 <br>
 - 함수의 경우 동사+명사 사용<br>
     - ex) getInformation()<br>
 - flag 변수는 조동사 + flag 종류로 구성 ([flag 변수란?](https://m.blog.naver.com/scyan2011/221610951335))<br>
     - ex) isNum<br>
 - 약어는 되도록 사용하지 않는다.
 </div>
 </details>

 <details>
 <summary>주석</summary>
 <div markdown="1">   
    
 - 한 줄 주석은 `//`를 사용한다.<br>
 - 그 이상은 `/** */`를 사용한다.
 </div>
 </details>

## Developers & 담당 업무
| 이름 | 포지션 | 담당 업무 |
| --- | --- | --- |
| 손민하 | 백앤드 / 팀장 | 제품, 주문, 배송 |
| 김은주 | 백앤드 | 회원가입, 게시판 |
| 윤현수 | 프론트 | 관리자, 회원가입, 로그인  |
| 장재우 | 프론트 | 장바구니,주문,레이아웃 |
