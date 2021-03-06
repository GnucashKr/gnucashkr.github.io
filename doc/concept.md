---
title: GnuCash 개요
---
## 장부(Book)
- 홍길동 가계부, (주)율도국 회계장부와 같은, 특정 주체/조직이 관리하는 계정 전체
- 여러 개의 계정으로 구성되며, 장부 하나가 GnuCash 파일 한 개에 저장됨

## 계정(Account)
- 은행계좌, 현금, 부채, 월급, 가스비 등, 연관된 거래를 묶어서 저장하는 기본 단위

### 계정 유형(Account Type)
- 계정마다 유형을 지정하여 계정의 성격에 맞게 관리할 수 있음
    - 가령, 입력기에서 입력할 수 있는 항목이 달라짐
    - '주식' 유형의 계정은 사거나 판 주식 수를 입력할 수 있다거나,
    - '신용카드' 유형의 계정은 계정 마감할 때 대금납부창을 띄우게 된다거나...
- 총 12개의 유형이 있음
    - 자산(Asset) 유형: 내가 보유한 것
        - 현금(Cash): 현금 및 외환
        - 은행(Bank): 자유입출금 및 예적금
        - 주식(Stock): 종목
        - 투자신탁(Mutual Fund): 펀드
        - 매출채권(Account Receivable): 미수금, 받을 어음
        - 일반자산(Other): 전세보증금, 빌려준 돈
    - 부채(Liability): 내가 빚진 것
        - 신용카드(Credit Card): 신용카드
        - 매입채무(Account Payable): 지급한 어음
        - 일반부채(Liability): 빌린 돈
    - 수입(Income): 내가 벌어들이는 것
    - 지출(Expense): 내가 쓰는 것
    - 자기자본(Equity): 자산 - 부채

### 계정 구조(Account hierarchy)
- 계정간의 폴더 구조라고 생각하면 편함
- 다른 계정을 포함하는 계정은 부모계정(Parent Account), 자식계정은 하위계정(Subaccount)
- 일반적인 직장인의 경우 아래와 같은 계정 구조를 가지게 될 것임
    - 자산
        - 입출금자유(은행 유형)
            - XX은행 OOO통장
            - YY은행 AAA통장
        - 주식(주식 유형)
            - OO텔레콤
            - AA자동차
        - 전세보증금(자산 유형)
    - 부채
        - 대출금(부채 유형)
        - 신용카드(신용카드 유형)
            - OO카드
            - AA카드
    - 수입
        - 급여(수입 유형)
            - 상여금(수입 유형)
        - 이자수입(수입 유형)
    - 지출
        - 식비(지출 유형)
        - 세금(제출 유형)
        - 의료비(지출 유형)
        - 주거비(지출 유형)
        - 통신비(지출 유형)

## 거래(Transaction)

### 입력기(Register)

### 부분거래(Split)

### 마감(Reconcile)

### 이체(Transfer)

### 예약(Schedule)

### 거래상태
- 신규(new)
- 확인(cleared)
- 마감(reconciled)
- 비어있음(void)

## 상품(Commodity)
- 상품 = 화폐 + 증권

### 화폐(Currency)

### 증권(Security)


- 비화폐상품(Non-currency commodity)라고도 부름

## 