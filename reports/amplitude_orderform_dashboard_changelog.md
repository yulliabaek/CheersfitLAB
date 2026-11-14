# 주문서 개선 결과 대시보드 변경 이력

대시보드: https://app.amplitude.com/analytics/cheersfitlab/dashboard/ez3qh535 (project 847753)

## 2026-11-14 — 퍼널 마지막 단계 변경
요청: 퍼널 마지막 단계를 Purchase(Web) 대신 주문완료 페이지 조회(/order/order_result.html)로 변경.

- 마지막 단계 정의: `[Amplitude] Page Viewed` where `[Amplitude] Page Path` contains `/order/order_result.html`
- 기간 유지: 분석 10/29~11/12 vs 비교 9/10~9/24 (Asia/Seoul, 15일, 동일 요일 구성), 전환 기간 1일, 테스트 계정 코호트(8j2y8rta) 제외

| 대시보드 위치 | 기존 차트 | 새 차트 |
|---|---|---|
| 주문서 진입 → 주문완료 퍼널 전환율 | oanjdjze | 24b5nimp |
| 주문서 진입 → 주문완료 일별 전환율 추이 | b0wt7eeb | htpvkql2 |
| 주문서 진입 → 주문완료 전환 소요 시간 분포 | w2jurz0s | 1a1eoiny (headline 뷰) |
| 결제 버튼 클릭 후 주문완료 전환율 | 21aszd65 | l7876gcx |
| 업셀 버튼 클릭 주문완료 전환 | 2iqbbitw | 0ys5qg9l |

변경 없음: 간편 결제 vs 일반 결제(8urkholy, Purchase의 order_place 기준), 평균 객단가(bulb7zsj, $revenue가 Purchase에만 있음).

### 결과 비교 (1일 전환)
| 퍼널 | 분석 기간 | 비교 기간 |
|---|---|---|
| 주문서 → Purchase(Web) (기존) | 63.3% (105/166) | 57.0% (122/214) |
| 주문서 → 주문완료 페이지 (변경) | 68.7% (114/166) | 61.9% (133/215) |
| 결제 버튼 → 주문완료 페이지 | 91.9% (113/123) | 86.4% (133/154) |
| 업셀 노출 → 클릭 → 주문완료 | control 8% (2/25), variant_a 0% (0/16) | — |
