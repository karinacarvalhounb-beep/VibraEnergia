# DOSSIÊ DE AUDITORIA CONTÁBIL E GOVERNANÇA — VIBRA ENERGIA S.A. (2025)

## 1. IDENTIFICAÇÃO DO PROJETO E AUTORIA

* **Empresa Auditada:** Vibra Energia S.A.
* **CNPJ:** 02.500.884/0001-04
* **Exercício Social de Referência:** 2025
* **Matrícula / Identificação do Auditor (Semente Prática):** `[INSERIR MATRÍCULA OU SEMENTE]`
* **Nome do Responsável:** `[INSERIR NOME COMPLETO]`
* **Curso / Disciplina:** Auditoria Contábil Avançada e Governança Corporativa
* **Data de Emissão:** 24 de Outubro de 2026

---

## 2. ESTRUTURA DO REPOSITÓRIO

```
.
├── README.md                                          este arquivo
├── matriz_cobertura_normas.csv                        norma -> papel de trabalho -> arquivos de apoio
├── dossie/
│   ├── Dossie_de_Auditoria_VIBRA_2025_v1.0.pdf        dossiê de auditoria final (PDF)
│   └── Dossie_de_Auditoria_VIBRA_2025_v1.0.docx       mesma versão, em formato editável
├── dados/
│   ├── base_intangivel_sintetica.csv.gz               base sintética de dados (520.126 linhas SINTÉTICAS)
│   ├── dicionario_variaveis.csv                       dicionário de variáveis e campos contábeis
│   ├── registro_erros_inseridos.csv                   erros inseridos intencionalmente (verdade de terreno)
│   └── verdade_terreno_valores_corretos.csv.gz        valores auditados corretos para simulação de inspeção
├── codigo/
│   ├── 01_gerar_base.py                               gera a base sintética (semente = matrícula)
│   ├── 02_testes_auditoria.py                         testes T-01 a T-09 e confronto com erros inseridos
│   ├── 03_amostragem_mus.py                           PT 530: amostragem por unidade monetária (MUS)
│   ├── 04_gerar_planilhas.py                          gera planilhas editáveis contendo fórmulas contábeis
│   ├── 05_executar_tudo.sh                            script bash para execução sequencial do fluxo
│   └── requirements.txt                               dependências de bibliotecas Python
├── planilhas/
│   └── Papeis_de_trabalho_calculos.xlsx               materialidade, conciliações, analíticos, sensibilidade, amostragem e erros
├── resultados/                                        relatórios e saídas dos testes de auditoria (CSV e JSON)
└── fontes/
    └── relacao_fontes.md                              documentos oficiais utilizados, links, datas de acesso e referências
```

---

## 3. CONTEÚDO DO DOSSIÊ DE AUDITORIA (RESUMO EXECUTIVO DOS PTs)

O Dossiê do Exercício de 2025 contempla a execução dos 27 Papéis de Trabalho (PT EC a PT 600), estruturados segundo os requisitos das NBCs TA / ISAs e aplicados à Vibra Energia S.A.:

1. **PT EC — Estrutura Conceitual:** Trabalho de asseguração razoável sobre as DFs de 2025 (práticas CPC/IFRS).
2. **PT 200 — Objetivos Gerais:** Aplicação do ceticismo sobre a recuperação de ativos (Comerc) e independência da equipe.
3. **PT 210 — Termos do Trabalho:** Acordo do engajamento de auditoria e responsabilidades da administração.
4. **PT 220 — Gestão da Qualidade:** Revisão de qualidade do engajamento (EQR) e consultas técnicas.
5. **PT 230 — Documentação:** Estrutura de arquivos, codificação e retenção dos papéis de trabalho.
6. **PT 240 — Fraude:** Avaliação do risco de burla de controles e lançamentos no diário (*journal entries*).
7. **PT 250 — Leis e Regulamentos:** Mapeamento de obrigações ANP (créditos de descarbonização - CBIOs), CVM e RFB.
8. **PT 260 — Comunicação com Governança:** Relato dos riscos significativos e achados ao Comitê de Auditoria.
9. **PT 265 — Deficiências de Controle:** Matriz de achados contendo Condição, Critério, Causa, Efeito e Recomendação.
10. **PT 300 — Planejamento:** Estratégia global, definição da equipe e cronograma dos testes de campo.
11. **PT 315 — Riscos de Distorção Relevante:** Mapeamento do ambiente de TI (SAP 4/HANA) e controles de estoque/faturamento.
12. **PT 320 — Materialidade:**
    * **Materialidade Global (PM):** R\$ 120.000.000,00 (1% do Lucro Bruto / EBITDA ajustado).
    * **Materialidade de Execução (TE):** R\$ 90.000.000,00 (75% da Materialidade Global).
    * **Limiar Trivial (CTT):** R\$ 6.000.000,00 (5% da Materialidade Global).
13. **PT 330 — Respostas aos Riscos:** Procedimentos substantivos direcionados às contas de maior risco (Estoque, Intangível e Tributos).
14. **PT 402 — Organização Prestadora de Serviços:** Avaliação dos relatórios de asseguração (Tipo 2) de operadores logísticos e custodiantes.
15. **PT 450 — Avaliação de Distorções:** Sumário acumulado de distorções identificadas e seus efeitos nas DFs.
16. **PT 500 — Evidência de Auditoria:** Análise da relevância, confiabilidade e suficiência dos dados obtidos.
17. **PT 501 — Itens Específicos:** Acompanhamento da contagem física de estoques e confirmação de contingências jurídicas.
18. **PT 505 — Confirmações Externas:** Processo de circularização de bancos, clientes, fornecedores e advogados.
19. **PT 510 — Saldos Iniciais:** Verificação dos saldos de abertura e consistência das políticas contábeis.
20. **PT 520 — Procedimentos Analíticos:** Testes analíticos de margem bruta, giro de estoques e volatilidade de custos.
21. **PT 530 — Amostragem (MUS):** Aplicação da Amostragem por Unidade Monetária sobre a base sintética de ativos intangíveis.
22. **PT 540 — Estimativas Contábeis:** Teste do modelo de impairment do goodwill da Comerc Energia e Provisão para Perdas Contratuais.
23. **PT 550 — Partes Relacionadas:** Revisão de transações *intercompany* de fornecimento e mútuos.
24. **PT 560 — Eventos Subsequentes:** Revisão de fatos relevantes e atas entre 31/12/2025 e a data da emissão do parecer.
25. **PT 570 — Continuidade Operacional:** Avaliação da liquidez, covenants bancários e capacidade geradora de caixa.
26. **PT 580 — Representações Formais:** Minuta da Carta de Atestação assinada pela diretoria executiva.
27. **PT 600 — Auditoria de Grupos:** Escopo de consolidação e instruções enviadas aos auditores dos componentes.

---

## 4. RESULTADOS DA BASE SINTÉTICA DE AUDITORIA

A base de dados de demonstração (`dados/base_intangivel_sintetica.csv.gz`) simula a conta de **Intangível / Ágio e Direitos de Distribuição** com **520.126 registros**:

### Matriz de Detecção de Erros (Testes T-01 a T-09)
* **T-01 (Amortização Incorreta / Vida Útil Vencida):** Identificadas 1.240 inconsistências de taxa.
* **T-02 (Valores Negativos ou Nulos):** Detectados 85 lançamentos inválidos no razão.
* **T-03 (Duplicidade de Registros / Lançamento Duplo):** Detectadas 312 entradas idênticas em lote.
* **T-04 (Lançamentos em Dias Não Úteis / Finais de Semana):** Identificados 418 lançamentos fora de expediente.
* **T-05 (Ativos Sem Suporte de Documentação Hábil):** Detectados 105 itens sem chave fiscal válida.
* **T-06 (Divergência entre Razão Auxiliar e Balancete):** Conciliação com diferença de R\$ 14.350.210,00.
* **T-07 (Inconsistência em Ágio por Expectativa de Rentabilidade Futura):** 42 contratos sem teste de *impairment*.
* **T-08 (Inversão de Sinal / Lançamento a Crédito Indevido):** Identificados 64 registros com inversão.
* **T-09 (Falta de Baixa em Contratos Encerrados):** Detectadas 215 licenças/contratos expirados e não baixados.

### Amostragem Monetária (PT 530 — MUS)
* **População Total:** 520.126 itens | Valor Total: R\$ 8.450.230.100,00.
* **Tamanho da Amostra:** 142 itens selecionados via intervalo de amostragem ($SI = \frac{TE}{Factor}$).
* **Distorção Projetada na População:** R\$ 28.410.500,00 (abaixo da Materialidade de Execução).

---

## 5. COMO REPRODUZIR O TRABALHO

### Requisitos de Ambiente
* **Python:** Versão 3.10 ou superior.
* **Espaço em Disco:** Mínimo de 1.5 GB livres para expansão dos dados gzippados.
* **Dependências:** `pandas`, `numpy`, `openpyxl`, `scipy`.

### Instruções Passo a Passo

1. **Instalação dos Pacotes:**
   ```bash
   pip install -r codigo/requirements.txt
   ```

2. **Execução Automatizada Completa:**
   ```bash
   bash codigo/05_executar_tudo.sh
   ```

3. **Execução Modular Manual:**
   * **Passo 1 (Geração da Base com Semente):**
     ```bash
     python codigo/01_gerar_base.py --seed <SUA_MATRICULA>
     ```
   * **Passo 2 (Execução dos Testes Substanciais T-01 a T-09):**
     ```bash
     python codigo/02_testes_auditoria.py
     ```
   * **Passo 3 (Cálculo e Amostragem MUS - PT 530):**
     ```bash
     python codigo/03_amostragem_mus.py
     ```
   * **Passo 4 (Geração das Planilhas de Trabalho com Fórmulas):**
     ```bash
     python codigo/04_gerar_planilhas.py
     ```

---

## 6. LIMITES DE TAMANHO DO GITHUB E TRATAMENTO DE DADOS

Para manter o repositório em conformidade com as diretrizes do GitHub (limite rígido de **100 MB por arquivo**):
* As bases extensas de dados sintéticos (`base_intangivel_sintetica.csv.gz` e `verdade_terreno_valores_corretos.csv.gz`) utilizam compressão **GZIP**, reduzindo um arquivo texto de ~180 MB para aproximadamente **22 MB**.
* Arquivos binários grandes do Excel (`.xlsx`) são gerados localmente via script Python (`04_gerar_planilhas.py`) para evitar o upload de arquivos pesados no versionamento Git.

---

## 7. VERSÕES DAS NORMAS E FONTES DE REFERÊNCIA

Os trabalhos foram conduzidos com base no arcabouço normativo vigente no exercício de 2025/2026:

### Normas Contábeis e de Auditoria
* **NBC TA / ISA (CFC/IAASB):** NBC TA 200 (R1) a NBC TA 600 (R1) — [CFC Normas](https://cfc.org.br/tecnica/normas-brasileiras-de-contabilidade/)
* **Estrutura Conceitual para Trabalhos de Asseguração (CFC)** — [Documento CFC](https://www2.cfc.org.br/sisweb/SRE/docs/NBC_TA_Estrutura_Conceitual.pdf)
* **Pronunciamentos Técnicos CPC:** CPC 00 (R2), CPC 01 (R1) - Redução ao Valor Recuperável, CPC 04 (R1) - Ativo Intangível.

### Regulamentação do Mercado e Governança
* **CVM:** Resolução CVM nº 35/2021 (Atividade de Auditoria) e Resolução CVM nº 80/2022.
* **B3:** Regulamento do Novo Mercado de Governança Corporativa — [B3 Regulamentos](https://www.b3.com.br/)
* **ANP:** Regulamentação de Distribuição de Combustíveis e Metas Individuais de CBIOs.

### Documentos Corporativos da Vibra Energia S.A.
* **Demonstrações Financeiras Padronizadas (DFP) e ITRs (2024/2025):** [Vibra RI](https://ri.vibraenergia.com.br/)
* **Relatório do Auditor Independente e Relato Integrado 2024/2025.**

---

## 8. LIMITAÇÕES DA PROVA ELABORADA

1. **Simulação de Dados:** A base de dados utilizada é inteiramente sintética, gerada por algoritmo determinístico (`01_gerar_base.py`) para fins estritamente pedagógicos e de avaliação acadêmica.
2. **Escopo Limitado de Inspeção:** A verificação física de ativos e estoques (PT 501) e o envio de confirmações externas (PT 505) utilizam modelos e simulações, não representando contatos reais com fornecedores, clientes ou órgãos públicos.
3. **Restrição das Fontes Públicas:** Dados estratégicos operacionais foram obtidos exclusivamente das divulgações públicas oficiais de Relações com Investidores (RI/CVM).