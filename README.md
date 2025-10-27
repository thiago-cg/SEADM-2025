# SEADM-2025 — Oficina ACTA → Design de Sistemas Multiagentes

Repositório criado para os materiais da **oficina** ministrada na **Semana Acadêmica de Administração 2025**.

Foco: aplicar **Applied Cognitive Task Analysis (ACTA)** — **Task Diagram Interview (TDI)** + **Knowledge Audit (KA)** — e converter achados em **A‑SPECs** (especificações de agentes) prontos para prototipagem.

> **Público‑alvo:** administradores e gestores (nível técnico ~4/10).
>
> **Proposta de valor:** conhecimento de negócio → **pré‑projeto de agentes** governável, auditável e acionável.

---

## 🔗 Materiais essenciais

* **Apresentação da oficina** → [Clique aqui](https://docs.google.com/presentation/d/1arZ31niw6eXplWi98n55VgYpco3U-ZHPbA5YpG_kmiw/edit?usp=sharing)
* **Roteiro de entrevistas** → [Clique aqui](https://docs.google.com/document/d/12LCiQjVcSFUqQ6uK2QXE6PdbUQnSQhCKUcocsgorj4I/edit?usp=sharing)
* **Planilha de TDI e KA** → [Clique aqui](https://docs.google.com/spreadsheets/d/13nsfSRa1U-zbv6XyV_0zwDCWnXy1740AH2y062i8TGI/edit?usp=sharing)
* **Gerador de A‑SPECs** → [Clique aqui](https://chatgpt.com/g/g-68f5521a3f848191b3427b6ff6aebc0c-gerador-de-a-specs)

---

## 🚀 Quickstart (15–30 min)

1. **Faça uma cópia** da *Planilha de TDI e KA*.
2. **Entrevista TDI (Task Diagram Interview):** descreva **3–6 passos**, com propósito, entradas/saídas (**formato obrigatório**), riscos e **carga cognitiva (1–5)**.
3. **Knowledge Audit:** para **2–3 passos “quentes”**, capture **episódios reais**, **cues/sinais**, **estratégias/heurísticas** e **erros de novatos**.
4. **Cole os dados** no **Gerador de A‑SPECs** e gere:

   * **Tabela A‑SPEC (Markdown)**
   * **JSON A‑SPEC** (com **contrato de I/O**, guardrails, KPIs, handoffs, privacy, etc.)
5. **Revise** com as rubricas de qualidade (checar formatos, LGPD, autonomia do agente) e ajuste antes do protótipo.

> **Dica de gestor:** *outputs sem formato = retrabalho*. Sempre especifique o **formato** (CSV/JSON/tabela) e o **destino** (ex.: “atualizar status no Jira”, “enviar e‑mail ao sponsor”).

---

## 🧩 Fluxo de trabalho (resumo executivo)

1. **Definir escopo da tarefa** (1 frase com verbo forte + contexto).
2. **TDI** (macroprocesso): passos, entradas/saídas (com **formato**), riscos, **carga 1–5**.
3. **KA** (profundidade): episódios reais, **cues**, heurísticas, erros típicos.
4. **Mapeamento → agentes**: *Planner / Router / RAG / Critic / Executor / Monitor*.
5. **Gerar A‑SPECs** (tabela e JSON) com **contratos de I/O** e **guardrails**.
6. **QA**: validações, LGPD, autonomia (0–3), KPIs e handoffs.
7. **Protótipo** (fora do escopo deste repo): implementar *o primeiro agente* com logs e aprovação humana.

---

## 🛠️ Boas práticas de engenharia de prompt (para gestores)

* **Uma intenção por prompt**, contexto estável no `system`, dados mutáveis no `user`.
* **Contrato de saída obrigatório** (JSON Schema/tabela com cabeçalhos fixos).
* **Critérios de aceitação** explícitos (completude, conformidade, tempos).
* **Rastreabilidade curta** (`racional_resumido`, `citacoes`, `alertas/lacunas`).
* **Crítico/Validador antes da entrega** (schema + regras de negócio + LGPD).
* **Autonomia do agente (0–3)** definida por risco/compliance e reversibilidade.

---

## 🔒 LGPD, ética e governança

* **Minimização de dados**: evite PII desnecessária; se houver, anonimizar/pseudonimizar.
* **Base legal** clara para qualquer dado pessoal; **retenção** definida.
* **Auditabilidade**: registre decisões automatizadas e **limites de autonomia**.
* **Aprovação humana** obrigatória em risco alto/compliance.

---

## 📚 Conteúdos de apoio (no repo)

* **Guias rápidos**: TDI em 20’, KA em 25’, rubrica de prontidão 0–3 para agentes.
* **Kits de prompt**: Entrevistador ACTA, Planner, RAG com citação, Critic/Validator, Router, Executor, Monitor.
* **Modelos de A‑SPEC**: tabela e JSON exemplares com comentários.

---

## 📝 Como citar

```
SEADM-2025 — Oficina Análise Cognitiva da Tarefa para Design de Sistemas Multiagentes.
Universidade de Brasília, Semana Acadêmica de Administração, 2025.
Disponível em: https://github.com/<org>/SEADM-2025
```

---

## 💬 Suporte e dúvidas

* Utilize a aba **Issues** para perguntas, sugestões e relatos.
* Para dúvidas rápidas em aula: ver **docs/FAQ.md** (adicione conforme surgirem perguntas frequentes).

---

**Nota final:** este repositório é propositalmente pragmático. Se a saída não tiver **formato** e **destino**, ela não existe — só parece.
