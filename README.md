# Zostań AI / Agent Engineerem

> Publiczny roadmap mojej drogi do zawodu AI/Agent Engineera.
> Repo jest otwarte z dwóch powodów: może się komuś przydać w nauce, a bardziej doświadczeni mogą podrzucić rady lub sugestie.

---

## Dlaczego ten roadmap?

Rynek AI zmienia się szybciej niż jakikolwiek inny obszar technologii. AI/Agent Engineer to rola, która dopiero krystalizuje się jako odrębny zawód — ktoś, kto nie tylko używa modeli językowych, ale także projektuje, integruje i utrzymuje systemy z nimi powiązane. Ten roadmap ma pomóc uporządkować naukę i praktykę.

---

## Roadmap

<details>
<summary><strong>🔄 Krok 0 — Przygotowanie (tutaj jestem)</strong></summary>

[Link do pełnego kroku](./roadmap/step%200%20-%20Przygotowanie)

Solidne fundamenty zanim przejdziesz dalej: matematyka, Python, podstawy ML, SQL, Generative AI, narzędzia deweloperskie. Bez tego kolejne kroki nie mają sensu.

</details>

<details>
<summary><strong>⏳ Krok 1 — Praca z LLM API i Prompt Engineering</strong></summary>

Nauka efektywnej komunikacji z modelami językowymi przez API (Anthropic, OpenAI). Zaawansowane techniki promptingu: chain-of-thought, few-shot, structured outputs. Zrozumienie jak modele "myślą" i jak przygotować dane wejściowe.

</details>

<details>
<summary><strong>⏳ Krok 2 — RAG (Retrieval-Augmented Generation)</strong></summary>

Budowanie systemów, które łączą wiedzę z zewnętrznych źródeł z możliwościami LLM. Embeddingi, wektorowe bazy danych, chunking, reranking. To fundament większości produkcyjnych aplikacji wykorzystujących LLM.

</details>

<details>
<summary><strong>⏳ Krok 3 — Praca nad modelami (tworzenie, trenowanie, doskonalenie, ocena)</strong></summary>

Ten krok skupia się na zrozumieniu i praktycznej pracy z samymi modelami — zarówno budową od zera (np. modele specyficzne dla zadania), jak i doskonaleniem istniejących modeli (fine-tuning, LoRA), oraz ich ocenie i walidacji.

Zakres przykładowych tematów:
- Zbieranie i przygotowanie danych: anotacje, czyszczenie, augmentacja, podział na zbiory treningowe walidacyjne i testowe.
- Metody trenowania i dostrajania: fine-tuning, few-shot, transfer learning, LoRA, parameter-efficient tuning.
- Architektury i frameworki: Transformer, pytorch, TensorFlow, Hugging Face ecosystems.
- Ewaluacja: metryki (accuracy, F1, BLEU, ROUGE, perplexity), walidacja krzyżowa, testy przeciwko błędom i przypadkom brzegowym.
- Analiza i interpretowalność: SHAP, LIME, błędy klasyfikacji, analiza przyczynowa.
- Bezpieczeństwo i bias: wykrywanie uprzedzeń, testy adversarialne, mitigacje.
- Optymalizacja i deployment modelu: praca nad inference speed, quantization, pruning, a także monitorowanie wydajności po wdrożeniu.

</details>

<details>
<summary><strong>⏳ Krok 4 — Budowanie Agentów AI</strong></summary>

Projektowanie i implementacja autonomicznych agentów: pętle agentowe (ReAct, plan-and-execute), narzędzia (tools/functions), pamięć agenta, obsługa błędów i retry logic. Pierwszy kontakt z frameworkami agentowymi.

</details>

<details>
<summary><strong>⏳ Krok 5 — Zaawansowane Systemy Multi-Agent</strong></summary>

Systemy złożone z wielu współpracujących agentów: orkiestracja, komunikacja między agentami, podział ról, human-in-the-loop. Frameworki: LangGraph, AutoGen, CrewAI. Ocena i ewaluacja agentów rozproszonych.

</details>

<details>
<summary><strong>⏳ Krok 6 — Produkcja i MLOps dla Agentów</strong></summary>

Wdrażanie agentów na produkcję: konteneryzacja (Docker), API, monitoring, logowanie, obserwowalność (tracing LLM calls), cost management, bezpieczeństwo i guardrails. CI/CD dla systemów AI.

</details>

<details>
<summary><strong>⏳ Krok 7 — Specjalizacja i Portfolio</strong></summary>

Wybór specjalizacji (np. agenty kodujące, agenty do analizy danych, agenty biznesowe), budowanie portfolio projektów, udział w open-source, dokumentowanie rozwiązań. Przygotowanie do rozmów kwalifikacyjnych.

</details>

---

## Status

| Krok | Temat | Status |
|------|-------|--------|
| 0 | Przygotowanie | `W toku` |
| 1 | LLM API i Prompt Engineering | `Nierozpoczęty` |
| 2 | RAG | `Nierozpoczęty` |
| 3 | Praca nad modelami (tworzenie, trenowanie, doskonalenie, ocena) | `Nierozpoczęty` |
| 4 | Budowanie Agentów AI | `Nierozpoczęty` |
| 5 | Zaawansowane Systemy Multi-Agent | `Nierozpoczęty` |
| 6 | Produkcja i MLOps | `Nierozpoczęty` |
| 7 | Specjalizacja i Portfolio | `Nierozpoczęty` |

---

## Masz sugestię?

Jeśli jesteś bardziej doświadczony i widzisz coś, co powinienem dodać, zmienić lub o czym powinienem wiedzieć — otwórz **Issue** lub **Pull Request**. Każda rada jest mile widziana.

---

*Ostatnia aktualizacja: 2026-02-20*
