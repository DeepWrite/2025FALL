---
title: 좋은 논증문의 구조 - tables
layout: home
nav_order: 79
parent: 강의내용
permalink: /lectures/lemma-tables/
---

# 좋은 논증문의 구조

<div style="text-align: center;">
  <img src="/lectures/lemma-theorem/good_argument_structure.png" width="80%" height="auto">
</div> <br>

## 도식 설명

* **Introduction (서론)**
  주제 제시 → 최종 주장(Theorem) 미리 예고 → 논증 단계(로드맵) 안내

* **Core Argument (본문)**
  여러 차례의 **Thesis(They Say) → Anti-thesis(I Say) → Lemma(부분 결론)** 과정을 거침

  * 각 Anti-thesis는 기존 학설/주장의 한계를 비판적으로 겨냥
  * 근거 제시 후 Lemma(부분 결론)로 정리
  * 누적된 Lemma들이 다음 단계의 토대를 형성

* **Synthesis (통합)**
  누적된 Lemma들을 결합하여 **최종 논증 구조** 완성

* **Conclusion (결론)**
  Theorem(최종 주장)을 힘 있게 재진술 → Lemma들이 어떻게 이를 뒷받침하는지 보여줌 → 함의 제시

👉 이 도해는 “좋은 논증문은 무작위 주장들의 나열이 아니라, 각 부분 결론(Lemma)이 서로 연결되어 최종 결론(Theorem)으로 수렴하는 구조”임을 강조합니다.


## 기타 시각자료

1. **Lemma→Theorem 사다리**
   “They Say → Anti-thesis(=Lemma) × n → Theorem” 흐름을 한 눈에 보여주는 핵심 개념도. 각 반론(anti-thesis)이 독립된 부분결론(Lemma)로 승격되고, 이것들이 종합되어 최종 결론(Theorem)으로 귀결되는 구조를 시각화했습니다.

<div style="text-align: center;">
  <img src="/lectures/lemma-theorem/01_lemma_theorem_ladder.png" width="80%" height="auto">
</div> <br>

2. **분야별 경로(사회과학 vs 인문학)**
   동일한 ‘They Say → I Say’ 구조가 사회과학(가설/모형 비판→실증근거→Lemma)과 인문학(재해석→근거 텍스트/맥락→Lemma)에서 어떻게 달리 전개되는지 분기 다이어그램으로 제시했습니다. 두 갈래가 아래의 Theorem에서 합류합니다.

<div style="text-align: center;">
  <img src="/lectures/lemma-theorem/02_discipline_pathways.png" width="80%" height="auto">
</div> <br>


3. **작성 워크시트(빈 표)**
   수업 활동용 빈 표. 각 행에 “Thesis(They Say) → Anti-thesis(I Say) → Evidence → Lemma”를 채워 넣게 되어 있어, 학생들이 자신의 논증 골격을 바로 설계할 수 있습니다. 프린트 배포용으로 적합합니다.

<div style="text-align: center;">
  <img src="/lectures/lemma-theorem/03_outline_planner.png" width="80%" height="auto">
</div> <br>


4. **사례 맵(전망이론 Prospect Theory)**
   “기대효용이론(Thesis) → 확실성효과/확률가중/손실회피(각 Anti-thesis→Lemma) → Prospect Theory(Theorem)”로 이어지는 대표 사회과학 사례를 흐름도로 정리했습니다. 수업 중 사례 설명용으로 좋습니다.

<div style="text-align: center;">
  <img src="/lectures/lemma-theorem/04_case_map_prospect_theory.png" width="80%" height="auto">
</div> <br>


5. **Do / Don’t 체크리스트**
   Anti-thesis를 Lemma로 만드는 실천 체크리스트(옳은 습관 vs 흔한 함정)를 표로 정리했습니다. 과제 피드백 기준으로도 활용 가능합니다.

<div style="text-align: center;">
  <img src="/lectures/lemma-theorem/05_checklist_do_dont.png" width="80%" height="auto">
</div> <br>


---

<!-- =========================================================
     좋은 논증문 구조 (They Say → I Say(anti-thesis) → Lemma … → Theorem)
     Just the Docs 호환: 페이지 내 HTML 블록로 바로 사용 가능
     ========================================================= -->
<style>
  .arg-diagram { --ink:#111; --muted:#6b7280; --accent:#1f6feb; --bg:#fff; }
  .arg-diagram { font-size:16px; line-height:1.5; margin: 1.25rem 0; }
  .arg-diagram .title { text-align:center; font-weight:700; font-size:1.35rem; margin-bottom: .75rem; }
  .arg-diagram .subtitle { text-align:center; color:var(--muted); margin:-.35rem 0 1.25rem; }

  .arg-diagram .grid {
    display:grid;
    grid-template-columns: 1fr;
    gap: 1rem;
  }

  /* Cards (boxes) */
  .arg-box {
    border:2px solid var(--ink);
    border-radius:14px;
    background:var(--bg);
    padding: .9rem 1rem;
  }
  .arg-box h3 { margin:.1rem 0 .35rem; font-size:1rem; }
  .arg-box .kicker {
    display:block; font-size:.8rem; letter-spacing:.04em; text-transform:uppercase;
    color:var(--muted); margin-bottom:.25rem; font-weight:600;
  }
  .arg-box.theorem { border-color:var(--accent); }
  .arg-box.theorem h3 { color:var(--accent); }
  .arg-box .small { font-size:.92rem; color:#1f2937; }
  .arg-box .hint { font-size:.85rem; color:var(--muted); margin-top:.25rem; }

  /* Lanes (They Say ↔ I Say) */
  .lane {
    display:grid;
    grid-template-columns: 1fr 40px 1fr;
    gap: .75rem 1rem;
    align-items:center;
  }
  .lane .arrow-right { text-align:center; font-size:1.3rem; }
  .connector {
    text-align:center; color:var(--muted); font-size:.95rem; margin:.15rem 0 .35rem;
  }
  .centered { grid-column: 1 / -1; }

  /* Responsive */
  @media (max-width: 799px) {
    .lane { grid-template-columns: 1fr; }
    .lane .arrow-right { display:none; }
  }

  /* Optional subtle separators */
  .sep { height:1px; background:rgba(0,0,0,.06); margin:.2rem 0 .75rem; }
</style>

<div class="arg-diagram">

  <div class="title">좋은 논증문 구조</div>
  <div class="subtitle">“They Say → I Say(anti-thesis) → Lemma(부분 결론)”을 누적하여 최종 결론(Theorem)로</div>

  <!-- 0) Introduction -->
  <div class="grid">
    <div class="arg-box centered">
      <span class="kicker">서론 (Introduction)</span>
      <h3>주제 제시 · 최종 주장(예고) · 전개 로드맵</h3>
      <div class="small">
        글의 문제의식과 맥락을 짧게 제시하고, 최종 결론(=Theorem)을 예고합니다.
        이어서 본문이 어떤 단계(레마들)로 전개될지 간단히 안내합니다.
      </div>
    </div>

    <!-- 1) Cycle 1 -->
    <div class="lane">
      <div class="arg-box">
        <span class="kicker">They Say · Thesis #1</span>
        <h3>기존 지배적 견해 · 전제</h3>
        <div class="small">문헌/통념에서 널리 수용되는 주장이나 핵심 가정(전제)을 공정하게 요약합니다.</div>
        <div class="hint">※ 스트로맨 금지: 상대 견해를 정확·공정하게 기술</div>
      </div>
      <div class="arrow-right" aria-hidden="true">➜</div>
      <div class="arg-box">
        <span class="kicker">I Say · Anti-thesis → Lemma #1</span>
        <h3>핵심 반논지 제시 후 근거로 부분 결론 도출</h3>
        <div class="small">
          “그러나/반대로/이 견해는 ~를 간과한다”와 같이 <b>정확히 겨냥한 반논지</b>를 제시하고,
          데이터·사례·논변으로 뒷받침하여 <b>부분 결론(Lemma #1)</b>을 명시적으로 정리합니다.
        </div>
      </div>
    </div>
    <div class="connector">▼ 다음 쟁점(Thesis #2)로 진행</div>

    <!-- 2) Cycle 2 -->
    <div class="lane">
      <div class="arg-box">
        <span class="kicker">They Say · Thesis #2</span>
        <h3>연동되는 두 번째 기존 주장</h3>
        <div class="small">첫 전제와 연결되거나, 그 결과로 따라오는 또 다른 통설/가정을 소개합니다.</div>
      </div>
      <div class="arrow-right" aria-hidden="true">➜</div>
      <div class="arg-box">
        <span class="kicker">I Say · Anti-thesis → Lemma #2</span>
        <h3>두 번째 반논지 → 두 번째 부분 결론</h3>
        <div class="small">
          반례·측정 결과·텍스트 근거 등으로 정밀하게 논증하여 <b>Lemma #2</b>를 도출합니다.
          <div class="hint">이전 Lemma와의 연결(전이 문장)로 누적 논증임을 분명히 합니다.</div>
        </div>
      </div>
    </div>
    <div class="connector">⋯ (필요 시 Thesis #3 → Lemma #3, … 반복)</div>

    <div class="sep"></div>

    <!-- 3) Synthesis -->
    <div class="arg-box centered">
      <span class="kicker">Synthesis · 통합</span>
      <h3>누적된 Lemma들을 논리적으로 결합</h3>
      <div class="small">
        각각의 부분 결론이 <b>서로 어떻게 결합되어</b> 하나의 강한 주장으로 귀결되는지 구조적으로 보여줍니다.
        “Lemma #1과 #2로부터 따라서 …”처럼 명시적으로 합성합니다.
      </div>
    </div>

    <!-- 4) Theorem -->
    <div class="arg-box theorem centered">
      <span class="kicker">Theorem · 최종 결론</span>
      <h3>누적 논증에 의해 뒷받침되는 최종 주장</h3>
      <div class="small">
        서론에서 예고했던 주장을 <b>더 정밀한 형식</b>으로 재진술하고, 어떤 Lemma들이 이를 지지하는지 요약합니다.
        필요하면 한계·함의·후속 과제도 간략히 제시합니다.
      </div>
    </div>

    <!-- 5) Conclusion -->
    <div class="arg-box centered">
      <span class="kicker">결론 (Conclusion)</span>
      <h3>요지 환기 · 함의 제시 · 다음 질문</h3>
      <div class="small">
        본문 누적 논증을 한 번 더 압축하여 상기시키고, 연구/해석의 함의와 다음 단계 질문을 제시합니다.
      </div>
    </div>
  </div>

  <!-- 접근성/프린트 친화적 요약 목록 -->
  <details style="margin-top: .75rem;">
    <summary><strong>텍스트 요약(접기/펼치기)</strong></summary>
    <ol>
      <li><strong>서론</strong>: 주제·문제의식, 최종 주장(예고), 전개 로드맵</li>
      <li><strong>본문-순환 1</strong>: They Say(Thesis #1) → I Say(Anti-thesis) → <em>Lemma #1</em></li>
      <li><strong>본문-순환 2</strong>: They Say(Thesis #2) → I Say(Anti-thesis) → <em>Lemma #2</em> (필요 시 반복)</li>
      <li><strong>통합</strong>: Lemma들을 논리적으로 결합하여 누적 논증 제시</li>
      <li><strong>Theorem</strong>: 최종 결론을 명확히 재진술(어떤 Lemma가 어떻게 지지하는지 표시)</li>
      <li><strong>결론</strong>: 요지 환기, 함의/한계/후속 과제</li>
    </ol>
  </details>
</div>


---

