# comunityProject

#화면구성
<img width="2407" height="1205" alt="image" src="https://github.com/user-attachments/assets/6c121185-6e8a-4395-9c5d-bdfdb03575fb" />


<img width="790" height="370" alt="image" src="https://github.com/user-attachments/assets/8ef1a3f1-ffdf-4930-930b-9f96737efb06" />

Spring MVC의 표준 패턴에 따라 `/admin/home` 요청을 처리하며,

`@Controller`와 `@Autowired`를 활용해 **의존성 주입**,

`Model`을 통해 **통계 데이터를 JSP에 전달**하고,

`@Slf4j` 로그로 디버깅 및 유지보수성도 확보한 컨트롤러입니다.

<img width="776" height="549" alt="image" src="https://github.com/user-attachments/assets/5b97e3cc-e744-4d1d-9a50-53ed761d7cb5" />

@Service어노테이션과 @Autowired를 활용해

**StatsMapper와 UploadController를 주입**

하고,

**StatsService 인터페이스를 구현하여**

콘서트 매출 데이터를 조회·반환하는

**서비스 계층 로직을 담당**

합니다.

<img width="914" height="389" alt="image" src="https://github.com/user-attachments/assets/90eae2c2-4513-4190-8b6a-9a60b75cf9b9" />

`<select id="concertSales">`는 티켓 판매 데이터를 조회하는 SQL로,

**ORDERS_DETAILS·ORDERS·TICKET 테이블을 조인**하고,

**정산일 기준 필터링** 및 `tk_vprice`가 있는 경우에만

**수량 × 가격으로 매출을 집계**하는 쿼리입니다.

`StatsVO` 리스트로 결과를 매핑합니다

#기술스택

