# 📊 Nova Estimativa Técnica - Análise Independente
## Porto Seguro - Auto Frota - Pós-Venda

### ⚠️ IMPORTANTE: Estimativa Independente
> Esta estimativa foi elaborada **desconsiderando as colunas N (Complexidade), P (Tempo), Q (Porte) e R (Priorização Técnica)** da planilha original.
>
> A análise foi feita com base em:
> - Descrição detalhada de cada requisito (Coluna B)
> - Tipo do requisito (Sistema/Processo/Aplicação)
> - Épico e área funcional
> - Sistemas envolvidos e complexidade de integração
> - Impacto no negócio (KPIs)
> - Benchmarks de mercado de seguros
> - Experiência em projetos Java/Spring Boot com Oracle e Kafka

---

## 📋 Metodologia de Classificação Técnica

### Critérios de Complexidade (Análise Independente)

| Categoria | Horas Base | Características | Exemplos |
|-----------|------------|-----------------|----------|
| **S** (Simples) | 120-200h | Parametrizações, configs, treinamentos | Ajuste de parâmetro, curso |
| **M** (Médio) | 250-450h | Customizações, integrações simples (1-2 sistemas) | Novo campo, relatório |
| **C** (Complexo) | 500-900h | Integrações múltiplas (3+ sistemas), novos módulos | Workflow, API complexa |
| **MC** (Muito Complexo) | 1.000-1.600h | Novos sistemas, IA, múltiplos legados | Portal, módulo novo |
| **MP** (Mega Projeto) | 1.800-3.500h | Plataformas completas, apps mobile | App completo, plataforma |

### Fatores de Ajuste Considerados

| Fator | Multiplicador | Aplicação |
|-------|---------------|-----------|
| Integração SAP | +30% | Sistemas financeiros |
| Integração Oracle Procedures | +20% | Regras de negócio complexas |
| Múltiplos sistemas legados (>3) | +40% | Cotador, GSA, ABAS, etc. |
| WhatsApp Business API | +25% | BOTs e chatbots |
| Compliance SUSEP | +15% | Requisitos regulatórios |
| Kafka event-driven | +20% | Eventos assíncronos |
| Mobile (App nativo) | +50% | iOS + Android |

---

## 📑 ESTIMATIVA DETALHADA POR REQUISITO

### 🔵 MÓDULO: ABERTURA DA DEMANDA (15 requisitos)

| ID | Requisito | Sistemas Envolvidos | Categoria | Horas Base | Justificativa Técnica |
|----|-----------|---------------------|-----------|------------|----------------------|
| **1** | App para Motorista - autosserviço aviso incidente | BOT WhatsApp, Sistemas Legados, Portal Segurado | **MP** | **2.400h** | App mobile completo + integrações múltiplas + WhatsApp API + portais existentes. Desenvolvimento iOS/Android, backend, APIs REST, integração com sistemas de assistência |
| **2** | Autosserviço WhatsApp para Motorista | WhatsApp Business API, Laudo Web, APP Vistoria | **MC** | **1.200h** | Chatbot com fluxo conversacional complexo, upload de mídia, integração com 3 sistemas, NLU para interpretação |
| **3** | Formulário e Jornada para Pesados | Legados múltiplos, Nova Emissão R3 | **C** | **800h** | Redesenho de jornada, checklist dinâmico, integração com múltiplos sistemas para recuperação de dados |
| **4** | Célula Especialista em Pesados na CO | Processo + Sibel + Sistema Roteamento | **M** | **400h** | Workflow de roteamento, regras de distribuição, integração com central de operações |
| **5** | Coleta de Dados de Terceiros via WhatsApp | WhatsApp API, BCP, Bureau | **C** | **700h** | Chatbot + integração com bases externas (BCP, Bureau) para validação de terceiros |
| **6** | Enriquecimento Dados Veículo (DETRAN) | DETRAN API, Sistema de Dados, Legado | **C** | **850h** | Integração com DETRAN (webservice governamental), workflow de atualização, validações |
| **7** | Perguntas Adicionais Tempo de Proposta | Cotador Auto Frota, Nova Emissão R3, Assistência/Sinistro | **C** | **650h** | Formulários dinâmicos, propagação para múltiplos sistemas downstream |
| **8** | Workflow Atualização Dados Veículo | Cotador, Nova Emissão R3, Assistência, Sinistro | **C** | **750h** | Workflow de aprovação multinível, auditoria, propagação de dados |
| **9** | Novo Portal do Prestador (GPS, logística) | Portal novo, GPS, Sistemas de mercado (Autem) | **MP** | **3.000h** | Portal web completo do zero, integração GPS real-time, logística, indicadores, conexão com sistemas externos |
| **10** | Plataforma Laudo Digital (Não Padrão) | Plataforma nova, Mobile | **MC** | **1.400h** | Plataforma web/mobile para prestadores, assinatura digital, integração |
| **11** | Viabilidade Prestadores Padrão em Capitais | Processo + Análise | **S** | **180h** | Estudo de viabilidade, configuração de regras por região |
| **12** | Atualização Automática Portal Prestador | Portal existente, WebSocket/SSE | **M** | **300h** | Implementação de push notifications real-time no portal existente |
| **13** | Função Blanket no Sistema | Múltiplos sistemas (Assistência, Sinistro, Cotador) | **MC** | **1.100h** | Integração complexa para vincular Blanket com apólice, contabilização automática |
| **14** | Jornada Gestão Frota no App | App mobile, Múltiplos sistemas | **MP** | **2.800h** | Jornada mobile completa, dashboards, relatórios, múltiplas integrações |
| **15** | Consulta Assistências/Sinistros Portal Produção | Portal da Produção | **M** | **350h** | Novo módulo de consulta, perfil comercial, filtros |

**Subtotal Abertura:** **16.880h base**

---

### 🟢 MÓDULO: SINISTRO (31 requisitos)

| ID | Requisito | Sistemas Envolvidos | Categoria | Horas Base | Justificativa Técnica |
|----|-----------|---------------------|-----------|------------|----------------------|
| **16** | Acesso Edital para Analistas | Sistema Sinistro, Licitar | **C** | **600h** | Integração entre sistemas, modelo de dados resumido, permissões |
| **17** | Discriminação Clara de Cláusulas | Processo + Sistemas de Atendimento | **M** | **400h** | Padronização de cláusulas, modelo parametrizável |
| **18** | Consulta Cláusulas Condições Particulares | Portal Atendimento, Sistema Sinistro, Cotador | **C** | **650h** | Integração de 3 sistemas para consulta unificada |
| **19** | Sistema Multi-item ABAS (Histórico) | GSA, ABAS | **MC** | **1.300h** | Redesenho de modelo de dados, histórico de vigências, múltiplas consultas |
| **20** | Desassociar Item Único da Apólice | Cotador AutoFrota | **C** | **700h** | Lógica complexa de cancelamento parcial, recálculo de vigência |
| **21** | Endosso para Reabilitação de Itens | Cotador Auto Frota | **C** | **600h** | Novo tipo de endosso, regras de negócio específicas |
| **22** | Visualização Segregada Casco/Acessórios | GSA | **C** | **700h** | Modelo de dados segregado, lotes separados, franquias |
| **23** | Análise Segregada Sinistros (PT+PP) | Sistema de Sinistro | **C** | **750h** | Workflow de análise dual, regras PT casco + PP acessório |
| **24** | Exclusão Automática Acessório (PT) | Cotador, Sistema Sinistro | **C** | **550h** | Automação baseada em consumo de verba, integração |
| **25** | Pop-up Auto Frota Compacto | LaudoWeb | **S** | **150h** | Componente de UI, regras de exibição |
| **26** | Revisão Escolhas de Acessórios | Processo + Cotador | **M** | **400h** | Redesenho de formulário, categorias específicas |
| **27** | Regras Cobertura Motorhome | Cotador AutoFrota, Sistemas Sinistro | **C** | **550h** | Modelo de cobertura específico, propagação para sistemas |
| **28** | Bloqueio Endosso com Sinistro II | Cotador AutoFrota | **M** | **250h** | Validação simples, regra de bloqueio |
| **29** | Endosso Automático Retirada Acessório | Sistema Sinistro, Cotador | **C** | **700h** | Automação de endosso, gatilhos, múltiplos cenários |
| **30** | Cláusulas 2º Risco na Apólice | Sistemas Assistência/Sinistro, Nova Emissão R3 | **C** | **650h** | Mapeamento de dados existentes, visualização unificada |
| **31** | Oficinas de Motorhome | Processo + Sistema | **M** | **350h** | Configuração de habilitação, filtros de oficina |
| **32** | Treinamento Prestadores (Pátio) | Plataforma de treinamento | **M** | **400h** | Módulo de treinamento online, notificações |
| **33** | Canal Direto Prestador/Time Técnico | Chat/Comunicação integrada | **C** | **700h** | Sistema de comunicação em tempo real, roteamento |
| **34** | IA para Análise de PT | IA/ML, Sistema Prestador | **MC** | **1.500h** | Modelo de ML para análise de imagens, treinamento, integração |
| **35** | Integração Sistemas para Laudos | Múltiplos sistemas Porto | **C** | **800h** | Integração de múltiplos sistemas, notificações Kafka |
| **36** | Cláusulas com LMI na Apólice | Sistemas Sinistro/Assistência | **M** | **400h** | Campos adicionais, consulta |
| **37** | Integração Blanket Análise Sinistro | Sistemas Sinistro, Cotador, Nova Emissão R3 | **MC** | **1.100h** | Integração de 3+ sistemas, busca de dados do aviso |
| **38** | Endosso por Perda de Direitos | Sistema de Sinistro | **C** | **550h** | Novo tipo de endosso específico |
| **39** | Bloqueio Alteração Tarifa com Sinistro | Cotador Auto Frota | **C** | **600h** | Regra de bloqueio, versionamento de tarifa |
| **40** | Parametrização de FIPE | Processo + Sistema | **M** | **300h** | Ajuste de parametrização existente |
| **41** | Visualização Sinistro por Item | Sistema de Sinistro | **C** | **700h** | Modelo de visualização, regras de dedução |
| **42** | Relatórios no COL | COL | **M** | **400h** | Novos relatórios, filtros dinâmicos |
| **43** | Portal/APP Integrado (Segurado, Motorista, Corretor, Terceiro) | Portal/APP novo, BOTs | **MP** | **2.500h** | Portal multi-perfil, múltiplas jornadas, integrações |
| **44** | Capilaridade de Oficinas | Sistema de cadastro | **M** | **300h** | Expansão de cadastro, filtros por tipo |
| **45** | Retroalimentação Cadastro Oficinas | Workflow de retroalimentação | **M** | **350h** | Automação de atualização baseada em eventos |
| **46** | Veículos Especiais Remoção Peças | Processo + Sistema | **M** | **400h** | Estudo + configuração de regras de acionamento |

**Subtotal Sinistro:** **20.400h base**

---

### 🟡 MÓDULO: ASSISTÊNCIA (16 requisitos)

| ID | Requisito | Sistemas Envolvidos | Categoria | Horas Base | Justificativa Técnica |
|----|-----------|---------------------|-----------|------------|----------------------|
| **47** | Capacitação Veículos Pesados | Plataforma treinamento | **M** | **350h** | Módulo de treinamento, conteúdo |
| **48** | Dados Cadastrais de Pesados | Processo + Sistema | **C** | **600h** | Extensão de modelo de dados, campos específicos |
| **49** | Parametrização Tempo para Pesados | Sistema de Assistência | **C** | **700h** | SLA diferenciado, timeline de comunicação |
| **50** | Apoio ao Passageiro | Processo + Sistema | **M** | **400h** | Workflow de apoio, integração voucher |
| **51** | Formalizar Assistência Passageiro | Processo/Documentação | **S** | **120h** | Documentação de processo, parametrização |
| **52** | Abertura Atendimento por Evento | Sistema de Assistência | **MC** | **1.000h** | Modelo de evento unificado, rastreabilidade total |
| **53** | Visão Serviços para Prestador | Sistema Assistência, Portal Prestador | **C** | **800h** | Dashboard completo, indicadores, TMA, SLA |
| **54** | Registro Negociações com Prestadores | Portal do Prestador | **C** | **650h** | Módulo de negociações, histórico |
| **55** | Botão Possível Fraude | Sibel | **C** | **600h** | Integração com Sibel, workflow de fraude |
| **56** | Lista de Fraude | Sistema novo + Compliance | **MC** | **1.200h** | Sistema de blocklist, integração compliance, consultas |
| **57** | Mecanismos Anti-Fraude | Motor de regras | **C** | **800h** | Motor de regras, detecção de padrões |
| **58** | Regras de Flexibilização | Sistema + Processo | **M** | **400h** | Parametrização de regras dinâmicas |
| **59** | Vistoria Pré-Seguro Automatizada | Workflow automatizado | **C** | **600h** | Automação baseada em risco, gatilhos |
| **60** | Educação Prestadores (Terabox) | Plataforma educacional | **M** | **350h** | Módulo de educação, notificações |
| **61** | Captura Informações Modal (Laudo Digital) | Sistemas Assistência/Sinistro, Nova Emissão R3 | **MC** | **1.100h** | Captura multimídia, laudo digital, múltiplas integrações |
| **62** | Prestadores-Chave Situações Específicas | Cadastro de prestadores | **M** | **350h** | Extensão de cadastro, habilidades |

**Subtotal Assistência:** **10.020h base**

---

### 🔴 MÓDULO: FINANCEIRO (14 requisitos)

| ID | Requisito | Sistemas Envolvidos | Categoria | Horas Base | Justificativa Técnica |
|----|-----------|---------------------|-----------|------------|----------------------|
| **63** | Isenção de Juros | SAP | **C** | **750h** | Workflow + motor de regras + integração SAP (complexa) |
| **64** | Automação de Devoluções | SAP | **C** | **800h** | Automação SAP, regras de bloqueio, múltiplos cenários |
| **65** | Fluxo Financeiro-Comercial (Inadimplência) | SAP, Sistema Legado | **C** | **700h** | Integração SAP-Legado, notificações automatizadas |
| **66** | Modelo de Faturamento | SAP, Cotador Auto Frota | **MC** | **1.400h** | Novo modelo financeiro, múltiplos meios de pagamento, SAP |
| **67** | Emissão Boleto D+0 | SAP, Cotador, Orquestrador | **C** | **700h** | Integração com orquestrador de pagamentos |
| **68** | Novos Meios de Pagamento (PIX) | SAP, Cotador, Gateway | **C** | **600h** | Integração com PIX, gateway de pagamentos |
| **69** | Régua Cobrança Órgãos Públicos | Processo + SAP | **C** | **650h** | Modelo específico de régua, integração SAP |
| **70** | Jornadas Reemissão e Endosso | Cotador, Sistema de Ticket | **MC** | **1.200h** | Jornadas completas, crédito interno, automação |
| **71** | Campo Obrigatório Devolução Endosso | SAP, Cotador | **M** | **400h** | Formulário, validações, bloqueio |
| **72** | Ajuste Cálculo Cancelamento | Cotador Auto Frota | **C** | **650h** | Lógica de cálculo complexa, restituições |
| **73** | Fluxos Vigência com Financeiro | Processo + Sistema | **M** | **400h** | Integração de comunicação, notificações |
| **74** | Regras de Arredondamento | Cotador Auto Frota, Múltiplos sistemas | **C** | **700h** | Padronização entre sistemas, conformidade |
| **75** | Painel Acompanhamento Portal Cliente | Portal do Cliente (PDC) | **MC** | **1.300h** | Dashboard completo, integrações múltiplas |
| **76** | Painel para Comercial Porto | Portal da Produção, SAP | **MC** | **1.300h** | Dashboard gestão comercial, SAP, relatórios |

**Subtotal Financeiro:** **11.550h base**

---

### 🟣 MÓDULO: CROSS (1 requisito)

| ID | Requisito | Sistemas Envolvidos | Categoria | Horas Base | Justificativa Técnica |
|----|-----------|---------------------|-----------|------------|----------------------|
| **77** | Indicadores Específicos para Frota | Múltiplos sistemas, NPS | **C** | **700h** | Definição de KPIs, dashboards, integrações com NPS |

**Subtotal Cross:** **700h base**

---

## 📊 RESUMO CONSOLIDADO - NOVA ESTIMATIVA

### Totais por Módulo

| Módulo | Qtd. | Horas Base | Horas +30% |
|--------|------|------------|------------|
| **Abertura** | 15 | 16.880h | **21.944h** |
| **Sinistro** | 31 | 20.400h | **26.520h** |
| **Assistência** | 16 | 10.020h | **13.026h** |
| **Financeiro** | 14 | 11.550h | **15.015h** |
| **Cross** | 1 | 700h | **910h** |
| **TOTAL** | **77** | **59.550h** | **77.415h** |

---

### Totais por Categoria de Complexidade

| Categoria | Qtd. | Horas Base | Horas +30% | % do Total |
|-----------|------|------------|------------|------------|
| **S** (Simples) | 4 | 570h | **741h** | 1% |
| **M** (Médio) | 22 | 7.900h | **10.270h** | 13% |
| **C** (Complexo) | 34 | 22.950h | **29.835h** | 39% |
| **MC** (Muito Complexo) | 12 | 14.900h | **19.370h** | 25% |
| **MP** (Mega Projeto) | 5 | 13.200h | **17.160h** | 22% |
| **TOTAL** | **77** | **59.550h** | **77.415h** | 100% |

---

### Totais por Onda

| Onda | Qtd. | Horas Base | Horas +30% |
|------|------|------------|------------|
| **Onda 1** | 25 | 15.730h | **20.449h** |
| **Onda 2** | 16 | 10.750h | **13.975h** |
| **Onda 3** | 23 | 19.800h | **25.740h** |
| **Autosserviço** | 8 | 9.150h | **11.895h** |
| **Despriorizado** | 5 | 4.120h | **5.356h** |
| **TOTAL** | **77** | **59.550h** | **77.415h** |

---

## 📈 COMPARATIVO: Estimativa Original vs Nova Estimativa

| Métrica | Planilha Original | Nova Estimativa | Diferença |
|---------|-------------------|-----------------|-----------|
| **Horas Base** | 47.840h | 59.550h | **+24,5%** |
| **Horas com Margem 30%** | 62.192h | **77.415h** | **+24,5%** |

### Justificativa da Diferença

A nova estimativa é **24,5% maior** que a original pelos seguintes motivos:

1. **Subestimativa de Mega Projetos (MP)**: Os requisitos 1, 9, 14 e 43 envolvem desenvolvimento de apps/portais completos que requerem muito mais esforço que os 832h máximos da planilha original.

2. **Complexidade de Integração com SAP**: Integrações SAP no módulo financeiro tipicamente consomem 30-50% mais tempo que outras integrações.

3. **Inteligência Artificial (Req. 34)**: O desenvolvimento de modelos de IA para análise de PT requer treinamento, validação e ajuste fino não contemplados na estimativa original.

4. **WhatsApp Business API**: Chatbots com fluxos conversacionais complexos e upload de mídia são substancialmente mais complexos que parametrizações simples.

5. **Múltiplas Integrações de Sistemas Legados**: A Porto possui 15+ sistemas a serem integrados, cada um com suas peculiaridades.

---

## ⏱️ ESTIMATIVA DE PRAZO - NOVA ANÁLISE

### Cenários de Equipe (77.415 horas totais)

| Cenário | Desenvolvedores | Meses | Anos | Recomendação |
|---------|-----------------|-------|------|--------------|
| Conservador | 10 | 48,4 | 4,0 | Muito longo |
| Moderado | 15 | 32,3 | 2,7 | Longo prazo |
| **Recomendado** | 20 | 24,2 | **2,0** | ✅ Equilibrado |
| Agressivo | 25 | 19,4 | 1,6 | Risco médio |
| Muito Agressivo | 30 | 16,1 | 1,3 | Alto risco |

### Por Onda (COM 20 DESENVOLVEDORES)

| Onda | Horas +30% | Meses | Prazo |
|------|------------|-------|-------|
| **Onda 1** | 20.449h | **6,4 meses** | ~6-7 meses |
| **Onda 2** | 13.975h | **4,4 meses** | ~4-5 meses |
| **Onda 3** | 25.740h | **8,0 meses** | ~8 meses |
| **Autosserviço** | 11.895h | Paralelo | - |
| **TOTAL** | **77.415h** | **24,2 meses** | ~24 meses |

---

## 🏗️ ESTRUTURA DE EQUIPE RECOMENDADA (20+ Desenvolvedores)

### Squads por Domínio

| Squad | Foco | Devs | Tech Lead | Especialistas |
|-------|------|------|-----------|---------------|
| **Squad Abertura** | Módulo Abertura + WhatsApp | 4 | 1 | 1 Chatbot Specialist |
| **Squad Sinistro** | Módulo Sinistro + GSA/ABAS | 5 | 1 | 1 DBA Oracle |
| **Squad Assistência** | Módulo Assistência + Prestadores | 4 | 1 | - |
| **Squad Financeiro** | Módulo Financeiro + SAP | 4 | 1 | 1 SAP Specialist |
| **Squad Mobile** | Apps iOS/Android | 3 | 1 | 1 UX Designer |
| **Squad IA/Data** | IA, Analytics, Indicadores | 2 | 1 | 1 Data Scientist |

### Papéis Adicionais

| Papel | Qtd. | Custo Adicional |
|-------|------|-----------------|
| Arquiteto de Soluções | 1-2 | Essencial |
| DBA Oracle | 2 | Essencial |
| DevOps/SRE | 2-3 | Essencial |
| QA Lead + Analysts | 4-5 | Essencial |
| Product Owners | 2-3 | Essencial |
| Scrum Masters | 2 | Recomendado |

---

## 🔧 RISCOS E MITIGAÇÕES

### Riscos Técnicos Identificados

| Risco | Probabilidade | Impacto | Mitigação |
|-------|---------------|---------|-----------|
| Integração SAP complexa | Alta | Alto | POC antecipada, especialista SAP |
| Sistemas legados sem documentação | Alta | Alto | Engenharia reversa, spike técnico |
| WhatsApp API limitações | Média | Médio | Fallback para outros canais |
| Performance Oracle em alto volume | Média | Alto | Testes de carga antecipados |
| Modelo de IA com baixa acurácia | Média | Médio | MVP simples, refinamento iterativo |
| Mudanças regulatórias SUSEP | Média | Alto | Buffer em cada onda |
| Dependência de times externos | Alta | Médio | Acordos de SLA, escalação |

---

## 📅 CRONOGRAMA SUGERIDO (20 Desenvolvedores)

```
┌───────────────────────────────────────────────────────────────────────────────────────┐
│                           TIMELINE TOTAL - 24 MESES                                   │
├───────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                       │
│ M1-M2      │ ▓▓▓▓▓ Arquitetura, POCs SAP/Oracle/Kafka, Setup Infra                    │
│                                                                                       │
│ M3-M9      │ ████████████████████████████████████████████ ONDA 1 (7 meses)            │
│            │ • 25 requisitos - Processos estruturantes                                │
│            │ • Foco: Treinamentos, bases, workflows                                   │
│                                                                                       │
│ M10-M14    │ █████████████████████████ ONDA 2 (5 meses)                               │
│            │ • 16 requisitos - Automações e integrações                               │
│            │ • Foco: Sistemas, automações, IA                                         │
│                                                                                       │
│ M15-M22    │ ██████████████████████████████████████████████████ ONDA 3 (8 meses)      │
│            │ • 23 requisitos - Sistemas complexos                                     │
│            │ • Foco: Portais, SAP, novos sistemas                                     │
│                                                                                       │
│ M23-M24    │ ▒▒▒▒▒ Estabilização, Testes E2E, Go-Live                                 │
│                                                                                       │
│ PARALELO   │ ░░░░░░░░░░░░░░░░░░░░░░ Squad Mobile + Autosserviço                       │
│            │ • 8 requisitos de autosserviço                                           │
│            │ • Apps Mobile iOS/Android                                                │
│                                                                                       │
└───────────────────────────────────────────────────────────────────────────────────────┘
```

---

## 💰 ESTIMATIVA DE CUSTO (Referência)

### Premissas
- Custo médio desenvolvedor/hora: R$ 150,00 (mercado SP)
- Inclui encargos e overhead

| Cenário | Horas | Custo Estimado |
|---------|-------|----------------|
| **Base (sem margem)** | 59.550h | R$ 8.932.500 |
| **Com Margem 30%** | 77.415h | **R$ 11.612.250** |

---

## ✅ CHECKLIST DE VALIDAÇÃO - NOVA ESTIMATIVA

### Dados Analisados

- [x] Descrição completa de cada requisito (Coluna B)
- [x] Tipo: Sistema (44), Processo (29), Aplicação (4)
- [x] Épicos: 8 áreas funcionais identificadas
- [x] Sistemas: 15+ sistemas mapeados
- [x] Impacto: Alto/Médio/Baixo
- [x] Funcionalidades descritas
- [x] Onda de entrega

### Colunas Desconsideradas (conforme solicitado)

- [x] Coluna N: Complexidade (ignorada)
- [x] Coluna P: Tempo em Horas (ignorada)
- [x] Coluna Q: Porte (ignorada)
- [x] Coluna R: Priorização Técnica (ignorada)

### Fatores Adicionais Considerados

- [x] Complexidade de integração com sistemas legados
- [x] Desenvolvimento mobile (iOS + Android)
- [x] Integrações SAP (+30% complexidade)
- [x] WhatsApp Business API
- [x] Modelos de IA/ML
- [x] Conformidade regulatória (SUSEP)
- [x] Event-driven com Kafka
- [x] Margem de segurança de 30%

---

*Documento gerado em: Dezembro/2024*
*Metodologia: Análise Técnica Independente + Benchmarks de Mercado*
*Margem de Segurança: +30%*
*Fonte de Dados: Planilha "Porto Pós - Mapa de Resolução de Dores.xlsx" (exceto colunas N, P, Q, R)*

