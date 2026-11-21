[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-00ff88?style=flat-square&logo=github)](https://tavardt-portugal.github.io/llm-robustness-evaluator-pt/)
[![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat-square&logo=python)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)
[![OWASP LLM](https://img.shields.io/badge/OWASP-LLM01%2FLLM02-red?style=flat-square)](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
[![NIST AI RMF](https://img.shields.io/badge/NIST-AI%20RMF-blue?style=flat-square)](https://www.nist.gov/artificial-intelligence)

<p align="center">
  <a href="https://ag.tavardt.com/pt/">
    <img src="https://ag.tavardt.com/img/tavardt-banner.png" alt="TAVARDT" width="600">
  </a>
</p>

# Avaliador de Robustez de LLM & Testador de Guardrails

**Auditoria Defensiva de Guardrails, Injeção de Prompt e Resiliência de Modelos de IA**

Ferramenta interativa e CLI defensiva para programadores avaliarem a robustez dos guardrails de LLMs contra vetores de injeção, fuga de prompt e ataques estruturais. Pontuação de Resiliência 0-100 + blueprint defensivo.

---

## Visão Geral

> **OWASP LLM01 & LLM02** | **NIST AI RMF** | **100% Defensive — Zero Offensive Payloads**

## 5 Vetores de Teste Defensivos

| # | Vector | Coverage |
|---|--------|----------|
| 1 | **Escape de Delimitador** — Detecta tokens de controle injetados (`</system>`, `[/INST]`, ` ``` `) | ✅ |
| 2 | **Vazamento de System Prompt** — Identifica padrões de extração de instruções do sistema | ✅ |
| 3 | **Substituição de Papel/Persona** — Verifica resistência a sobreposições (DAN, modo dev) | ✅ |
| 4 | **Ofuscação Estrutural** — Avalia cobertura contra Base64, leetspeak, homóglifos Unicode | ✅ |
| 5 | **Injeção Indireta de Contexto** — Simula documento RAG com payload embutido | ✅ |

---

## Ferramenta Online

Acesse a ferramenta interativa diretamente:

🌐 **[https://tavardt-portugal.github.io/llm-robustness-evaluator-pt/](https://tavardt-portugal.github.io/llm-robustness-evaluator-pt/)**

🛠 **[https://tools.tavardt.com/pt/](https://tools.tavardt.com/pt/)**

---

## Uso via CLI

### Instalação

```bash
git clone https://github.com/TAVARDT-Portugal/llm-robustness-evaluator-pt.git
cd llm-robustness-evaluator-pt
pip install -r requirements.txt
```

### Execução

```bash
python llm_robustness_evaluator.py --prompt "You are a helpful assistant."
```

```
Resilience Score: 85/100
✅ V1 Delimiter Escape — PASS
✅ V2 System Prompt Leakage — PASS
✅ V3 Role/Persona Override — PASS
✅ V4 Structural Obfuscation — PASS
⚠️  V5 Indirect Context Injection — WARNING
```

---

## Arquitetura Defensiva

O blueprint defensivo inclui:

- 🐍 Filtro Python para detecção de padrões de injeção
- 📦 Middleware TypeScript para APIs Next.js
- 🔒 Template de System Prompt reforçado com delimitadores imutáveis

---

## Portais Oficiais

Acesse a rede oficial de portais TAVARDT:

| Portal | URL |
|--------|-----|
| Portal Oficial TAVARDT | [https://ag.tavardt.com/pt/](https://ag.tavardt.com/pt/) |
| Central de Ferramentas | [https://tools.tavardt.com/pt/](https://tools.tavardt.com/pt/) |
| Contato | [https://ag.tavardt.com/pt/contact/](https://ag.tavardt.com/pt/contact/) |
| GitHub | [https://github.com/TAVARDT-Portugal](https://github.com/TAVARDT-Portugal) |

---

## Licença

MIT License — uso livre para fins defensivos e educacionais.

---

<p align="center">
  <strong>TAVARDT — Portugal</strong><br>
  <a href="https://ag.tavardt.com/pt/">https://ag.tavardt.com/pt/</a> &bull;
  <a href="https://tools.tavardt.com/pt/">https://tools.tavardt.com/pt/</a><br>
  &copy; 2025 TAVARDT. Todos os direitos reservados.
</p>
