# Smart_Contract_Assembly

EVM assembly 기반 ERC20/ERC721 학습용 예제 저장소입니다.

## 경고

이 코드는 교육 목적입니다.
메모리 안전성과 보안 취약점 가능성이 있으므로 운영 환경에서 사용하면 안 됩니다.

## 포함 파일

- `ERC20_Assem.sol`
  - assembly로 `name`, `symbol`, `totalSupply`, `balanceOf`, `mint`를 구현한 예제
- `ERC721_Assem.sol`
  - assembly 중심으로 `ownerOf`, `balanceOf`, `approve`, `transferFrom`, `_mint`, `_burn` 등을 구현한 예제

## 컴파일 참고

- `ERC20_Assem.sol`: Solidity `^0.8.18`
- `ERC721_Assem.sol`: Solidity `>=0.8.0`

## 학습 포인트

- 슬롯 직접 계산과 `sload`/`sstore` 사용 방식
- 이벤트 로그를 `log4`로 직접 기록하는 방식
- 잘못 구현하면 발생하는 메모리/권한/슬롯 충돌 리스크
