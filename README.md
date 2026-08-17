# Bistro Cupid 2 한국어 패치

PS2용 **Bistro Cupid 2 (Japan) (Tokubetsu-ban)** 전용 비공식 한국어 패치입니다.

이 저장소와 릴리스에는 원본 게임 ISO가 포함되어 있지 않습니다. 정품에서 직접 추출한, 아래 해시와 정확히 일치하는 ISO에 xdelta 패치를 적용해야 합니다.

## 지원 원본

- 파일명: `Bistro Cupid 2 (Japan) (Tokubetsu-ban).iso`
- 파일 크기: `2,296,709,120 bytes`
- SHA-256: `89C7380F6BC1906FDCF9DBAE2A6C28A6194A9642A924C58A619B0588EC6EB5CF`

## 적용 방법

릴리스에서 다음 두 파일을 받습니다.

- `Bistro Cupid 2 (Japan) (Tokubetsu-ban) [Korean].xdelta`
- `Bistro Cupid 2 (Japan) (Tokubetsu-ban) [Korean] - 적용 방법.txt`

xdelta3 명령줄 예시:

```text
xdelta3.exe -d -s "Bistro Cupid 2 (Japan) (Tokubetsu-ban).iso" "Bistro Cupid 2 (Japan) (Tokubetsu-ban) [Korean].xdelta" "Bistro Cupid 2 (Japan) (Tokubetsu-ban) [Korean].iso"
```

정상 적용 결과:

- 파일 크기: `2,296,709,120 bytes`
- SHA-256: `51EB59F10CC7DB775BDAEC299D8B0D6B3F8B50AF480D934EB96D2B3271BB95D5`

## 패치 범위

- 본편 대사, 화자명, 선택지 및 일본판에 없는 추가 스크립트
- 타이틀, 메인 메뉴, 설정, 세이브/로드, 앨범, 뮤직박스
- 일정, 상태, 경영, 영업 기록, 연구, 요리 목록과 설명
- 인테리어/물품 구매 설명과 관리 화면
- 캐릭터 이름과 상태 화면 도움말
- 전투/RPG 화면, 마법 이름과 설명
- 요일 및 기타 시스템 UI

자세한 범위는 [PATCH_SCOPE.md](PATCH_SCOPE.md)를 확인하세요.

## 제외 범위

- 오프닝·엔딩 영상 및 영상 안의 자막/이미지는 원본 그대로입니다.

## PCSX2 주의사항

패치 적용 전 만든 PCSX2 세이브스테이트를 불러오면 이전 실행 파일의 메모리가 복원되어 일부 도움말이 일본어로 나타날 수 있습니다.

1. 패치된 ISO를 완전히 새로 부팅합니다.
2. 게임 내 세이브 데이터로 `이어하기`를 선택합니다.
3. 새로 부팅한 뒤 세이브스테이트를 다시 만듭니다.

## 배포 안내

비상업적 팬 번역 패치입니다. 원본 ISO나 게임 데이터 전체를 재배포하지 마세요.

