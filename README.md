# Avaliador de Robustez e Resiliência de Modelos LLM

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-5b3cf5.svg)](https://tavardt-portugal.github.io/llm-robustness-evaluator-pt/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Robustness](https://img.shields.io/badge/Benchmarking-Robustness-orange.svg)](https://ag.tavardt.com/pt/)
[![NIST AI](https://img.shields.io/badge/NIST-AI%20RMF-blue.svg)](https://www.nist.gov/itl/ai-risk-management-framework)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

**Framework de Testes de Stress, Verificação de Estabilidade e Análise de Consistência de Respostas em Modelos de Linguagem**

Desenvolvido e mantido pela divisão de auditoria e garantia de qualidade em IA da TAVARDT Portugal.

***

## Portais e Demonstração Online

Aceda à ferramenta interativa oficial e aos canais soberanos da TAVARDT:

* **Aplicação Web Oficial no GitHub Pages**: [https://tavardt-portugal.github.io/llm-robustness-evaluator-pt/](https://tavardt-portugal.github.io/llm-robustness-evaluator-pt/)
* **Portal Institucional**: [https://ag.tavardt.com/pt/](https://ag.tavardt.com/pt/)
* **Central de Ferramentas**: [https://tools.tavardt.com/pt/](https://tools.tavardt.com/pt/)

***

## Blueprints Técnicos e Recursos Disponíveis

1. **Aplicação Web Interativa**: Diagnóstico determinístico, cálculo de postura defensiva e recomendações imediatas no navegador.
2. **Utilitário CLI Local**: Script Python determinístico executado diretamente no ambiente de produção para auditoria offline.
3. **Especificações de Segurança**: Manifestos e configurações de hardening em conformidade com as normas internacionais.

***

## Uso do Utilitário CLI Determinístico

Para executar a inspeção técnica no ambiente local:

```bash
git clone https://github.com/TAVARDT-Portugal/llm-robustness-evaluator-pt.git
cd llm-robustness-evaluator-pt
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python3 scanner.py -json
```

***

## Governança e Conformidade

* **Organização**: TAVARDT-Portugal
* **Jurisdição**: Portugal
* **Padrões de Referência**: Normas e frameworks técnicos auditados em estrita observância das regras de soberania.

Desenvolvido pela Divisão de Cibersegurança e Infraestrutura da TAVARDT Portugal. Todos os direitos reservados.

***

© 2026 TAVARDT Portugal. Todos os direitos reservados. Soberania e Defesa de Infraestrutura.
