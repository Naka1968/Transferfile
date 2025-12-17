# 📊 Estimativa Detalhada de Desenvolvimento
## Porto Seguro - Auto Frota - Pós-Venda

### Contexto do Projeto
- **Plataforma**: Java + Spring Boot
- **Banco de Dados**: Oracle
- **Mensageria**: Apache Kafka
- **Domínio**: Seguro de Frotas de Veículos (Carros e Caminhões)
- **Jornada**: Pós-Venda (Abertura, Assistência, Sinistro, Financeiro)

---

## ⚠️ MARGEM DE SEGURANÇA APLICADA: +30%

> Todas as estimativas incluem uma **margem de segurança de 30%** para cobrir:
> - Riscos de integração com sistemas legados
> - Complexidade não prevista em regras de negócio
> - Curva de aprendizado da equipe
> - Débito técnico e refatorações
> - Dependências externas e bloqueios
> - Ajustes de escopo durante o desenvolvimento

---

## 📋 Metodologia de Estimativa

### Critérios SDLC Aplicados

As estimativas consideram todas as fases do ciclo de desenvolvimento de software:

| Fase | % do Tempo Total | Atividades |
|------|------------------|------------|
| **Arquitetura & Design** | 15% | Desenho técnico, modelagem de dados, definição de APIs, documentação técnica |
| **Engenharia & Análise** | 20% | Refinamento de requisitos, análise de impacto, POCs, integração com sistemas legados |
| **Desenvolvimento** | 40% | Codificação, code review, refatoração, implementação de regras de negócio |
| **Testes** | 20% | Testes unitários, integração, e2e, performance, UAT |
| **Deploy & Documentação** | 5% | CI/CD, documentação de usuário, handoff |

### Classificação de Porte (Conforme Planilha Original)

| Porte | Horas Base | Horas com Margem 30% | Perfil |
|-------|------------|----------------------|--------|
| **P** (Pequeno) | 208h | **270h** | Parametrização simples, ajustes pontuais |
| **M** (Médio) | 416h | **541h** | Customizações moderadas, integrações simples |
| **G** (Grande) | 624h | **811h** | Desenvolvimento de funcionalidades completas |
| **GG** (Muito Grande) | 832h | **1.082h** | Sistemas novos, integrações complexas, múltiplos módulos |

---

## 📊 RESUMO EXECUTIVO - NÚMEROS ATUALIZADOS

### Totais Gerais

| Métrica | Valor Base (Planilha) | Com Margem 30% |
|---------|----------------------|----------------|
| **Total de Requisitos** | 77 | 77 |
| **Total de Horas** | 47.840h | **62.192h** |

---

## 📑 Estimativa Detalhada por Requisito (COM MARGEM 30%)

### 🔵 MÓDULO: ABERTURA DA DEMANDA

| ID | Requisito | Tipo | Porte | Complexidade | Horas Base | Horas +30% | Onda |
|----|-----------|------|-------|--------------|------------|------------|------|
| 1 | App para Motorista - autosserviço para aviso de incidente | Sistema | G | Alta | 624h | **811h** | Autosserviço |
| 2 | Autosserviço WhatsApp para Motorista | Sistema | G | Média | 624h | **811h** | Autosserviço |
| 3 | Formulário e Jornada para Pesados | Processo | GG | Média | 832h | **1.082h** | Onda 1 |
| 4 | Célula Especialista em Pesados na CO | Processo | G | Média | 624h | **811h** | Onda 1 |
| 5 | Coleta de Dados de Terceiros via WhatsApp | Sistema | G | Baixa | 624h | **811h** | Autosserviço |
| 6 | Enriquecimento de Dados do Veículo (DETRAN) | Sistema | G | Média | 624h | **811h** | Onda 3 |
| 7 | Perguntas Adicionais em Tempo de Proposta | Sistema | G | Média | 624h | **811h** | Onda 3 |
| 8 | Workflow de Atualização de Dados do Veículo | Sistema | G | Média | 624h | **811h** | Onda 3 |
| 9 | Novo Portal do Prestador (GPS, logística, indicadores) | Aplicação | GG | Alta | 832h | **1.082h** | Onda 3 |
| 10 | Plataforma de Laudo Digital (Prestadores Não Padrão) | Aplicação | GG | Média | 832h | **1.082h** | Onda 3 |
| 11 | Viabilidade de Prestadores Padrão em Capitais | Processo | G | Média | 624h | **811h** | Onda 1 |
| 12 | Atualização Automática do Portal do Prestador | Aplicação | P | Média | 208h | **270h** | Onda 1 |
| 13 | Função Blanket no Sistema | Sistema | GG | Média | 832h | **1.082h** | Onda 3 |
| 14 | Jornada Completa de Gestão de Frota no App | Aplicação | GG | Alta | 832h | **1.082h** | Onda 3 |
| 15 | Consulta de Assistências e Sinistros no Portal da Produção | Sistema | M | Média | 416h | **541h** | Autosserviço |

**Subtotal Abertura:** 9.776h base → **12.709h** com margem

---

### 🟢 MÓDULO: SINISTRO

| ID | Requisito | Tipo | Porte | Complexidade | Horas Base | Horas +30% | Onda |
|----|-----------|------|-------|--------------|------------|------------|------|
| 16 | Acesso ao Edital para Analistas de Sinistro | Sistema | G | Média | 624h | **811h** | Onda 2 |
| 17 | Discriminação Clara de Cláusulas | Processo | G | Média | 624h | **811h** | Onda 1 |
| 18 | Consulta de Cláusulas de Condições Particulares | Sistema | G | Média | 624h | **811h** | Autosserviço |
| 19 | Sistema Multi-item no ABAS (Histórico Apólice) | Sistema | GG | Média | 832h | **1.082h** | Onda 3 |
| 20 | Desassociar Item Único da Apólice | Sistema | G | Média | 624h | **811h** | Onda 2 |
| 21 | Endosso para Reabilitação de Itens | Sistema | M | Alta | 416h | **541h** | Onda 2 |
| 22 | Visualização Segregada Casco/Acessórios (GSA) | Sistema | G | Alta | 624h | **811h** | Onda 2 |
| 23 | Análise Segregada de Sinistros (PT Casco + PP Acessório) | Sistema | G | Alta | 624h | **811h** | Onda 2 |
| 24 | Exclusão Automática de Acessório (PT) | Sistema | G | Média | 624h | **811h** | Onda 3 |
| 25 | Pop-up Auto Frota Compacto (Cobertura PNR) | Sistema | M | Baixa | 416h | **541h** | Onda 3 |
| 26 | Revisão de Escolhas de Acessórios | Processo | G | Alta | 624h | **811h** | Onda 1 |
| 27 | Regras de Cobertura para Motorhome | Processo | G | Média | 624h | **811h** | Onda 1 |
| 28 | Bloqueio de Endosso com Sinistro II | Sistema | P | Baixa | 208h | **270h** | Onda 1 |
| 29 | Endosso Automático para Retirada de Acessório | Sistema | G | Alta | 624h | **811h** | Onda 3 |
| 30 | Cláusulas de 2º Risco na Apólice | Sistema | G | Média | 624h | **811h** | Onda 3 |
| 31 | Oficinas de Motorhome | Processo | G | Média | 624h | **811h** | Onda 1 |
| 32 | Treinamento de Prestadores (Veículos para Pátio) | Processo | G | Média | 624h | **811h** | Onda 1 |
| 33 | Canal Direto Prestador/Time Técnico | Processo | G | Alta | 624h | **811h** | Onda 1 |
| 34 | IA para Análise de PT | Sistema | G | Alta | 624h | **811h** | Onda 2 |
| 35 | Integração de Sistemas para Laudos | Processo | G | Alta | 624h | **811h** | Onda 1 |
| 36 | Cláusulas com LMI na Apólice | Sistema | G | Média | 624h | **811h** | Onda 3 |
| 37 | Integração Blanket para Análise de Sinistro | Sistema | GG | Média | 832h | **1.082h** | Onda 3 |
| 38 | Endosso por Perda de Direitos | Sistema | G | Alta | 624h | **811h** | Despriorizado |
| 39 | Bloqueio de Alteração de Tarifa com Sinistro Aberto | Sistema | G | Média | 624h | **811h** | Onda 2 |
| 40 | Parametrização de FIPE | Processo | M | Média | 416h | **541h** | Onda 1 |
| 41 | Visualização de Sinistro por Item | Sistema | G | Alta | 624h | **811h** | Onda 2 |
| 42 | Relatórios no COL | Sistema | M | Média | 416h | **541h** | Autosserviço |
| 43 | Portal/APP Integrado (Segurado, Motorista, Corretor, Terceiro) | Processo | G | Alta | 624h | **811h** | Onda 1 |
| 44 | Capilaridade de Oficinas | Processo | M | Média | 416h | **541h** | Onda 1 |
| 45 | Retroalimentação do Cadastro de Oficinas | Processo | M | Média | 416h | **541h** | Onda 1 |
| 46 | Veículos Especiais para Remoção de Peças | Processo | G | Alta | 624h | **811h** | Onda 1 |

**Subtotal Sinistro:** 18.512h base → **24.066h** com margem

---

### 🟡 MÓDULO: ASSISTÊNCIA

| ID | Requisito | Tipo | Porte | Complexidade | Horas Base | Horas +30% | Onda |
|----|-----------|------|-------|--------------|------------|------------|------|
| 47 | Capacitação para Veículos Pesados | Processo | G | Baixa | 624h | **811h** | Onda 1 |
| 48 | Dados Cadastrais de Pesados | Processo | G | Média | 624h | **811h** | Onda 2 |
| 49 | Parametrização de Tempo para Pesados | Sistema | G | Alta | 624h | **811h** | Onda 2 |
| 50 | Apoio ao Passageiro | Processo | G | Média | 624h | **811h** | Despriorizado |
| 51 | Formalizar Assistência ao Passageiro | Processo | P | Baixa | 208h | **270h** | Onda 2 |
| 52 | Abertura de Atendimento por Evento | Sistema | G | Alta | 624h | **811h** | Onda 2 |
| 53 | Visão de Serviços para Prestador | Sistema | G | Alta | 624h | **811h** | Onda 2 |
| 54 | Registro de Negociações com Prestadores | Sistema | G | Alta | 624h | **811h** | Onda 2 |
| 55 | Botão de Possível Fraude | Processo | G | Média | 624h | **811h** | Onda 1 |
| 56 | Lista de Fraude | Processo | GG | Baixa | 832h | **1.082h** | Onda 3 |
| 57 | Mecanismos Anti-Fraude | Processo | G | Média | 624h | **811h** | Onda 1 |
| 58 | Regras de Flexibilização | Processo | G | Média | 624h | **811h** | Onda 1 |
| 59 | Vistoria Pré-Seguro Automatizada | Processo | G | Média | 624h | **811h** | Onda 1 |
| 60 | Educação de Prestadores (Terabox) | Processo | G | Baixa | 624h | **811h** | Onda 1 |
| 61 | Captura de Informações para Modal (Laudo Digital) | Sistema | GG | Média | 832h | **1.082h** | Onda 3 |
| 62 | Prestadores-Chave para Situações Específicas | Processo | G | Média | 624h | **811h** | Despriorizado |

**Subtotal Assistência:** 9.984h base → **12.979h** com margem

---

### 🔴 MÓDULO: FINANCEIRO

| ID | Requisito | Tipo | Porte | Complexidade | Horas Base | Horas +30% | Onda |
|----|-----------|------|-------|--------------|------------|------------|------|
| 63 | Isenção de Juros | Sistema | G | Alta | 624h | **811h** | Onda 3 |
| 64 | Automação de Devoluções | Sistema | G | Alta | 624h | **811h** | Onda 2 |
| 65 | Fluxo Financeiro-Comercial (Inadimplência) | Sistema | G | Alta | 624h | **811h** | Onda 3 |
| 66 | Modelo de Faturamento | Sistema | GG | Alta | 832h | **1.082h** | Onda 3 |
| 67 | Emissão de Boleto D+0 | Sistema | G | Média | 624h | **811h** | Onda 3 |
| 68 | Novos Meios de Pagamento (PIX) | Sistema | M | Média | 416h | **541h** | Onda 3 |
| 69 | Régua de Cobrança para Órgãos Públicos | Processo | G | Alta | 624h | **811h** | Onda 1 |
| 70 | Jornadas de Reemissão e Endosso | Sistema | GG | Alta | 832h | **1.082h** | Onda 3 |
| 71 | Campo Obrigatório de Devolução no Endosso | Sistema | G | Média | 624h | **811h** | Onda 3 |
| 72 | Ajuste de Cálculo de Cancelamento | Sistema | G | Alta | 624h | **811h** | Despriorizado |
| 73 | Fluxos de Vigência com Financeiro | Processo | G | Média | 624h | **811h** | Despriorizado |
| 74 | Regras de Arredondamento | Sistema | G | Alta | 624h | **811h** | Onda 2 |
| 75 | Painel de Acompanhamento no Portal do Cliente | Sistema | GG | Alta | 832h | **1.082h** | Autosserviço |
| 76 | Painel para Comercial Porto | Sistema | GG | Alta | 832h | **1.082h** | Autosserviço |

**Subtotal Financeiro:** 8.960h base → **11.648h** com margem

---

### 🟣 MÓDULO: CROSS

| ID | Requisito | Tipo | Porte | Complexidade | Horas Base | Horas +30% | Onda |
|----|-----------|------|-------|--------------|------------|------------|------|
| 77 | Indicadores Específicos para Frota | Processo | G | Alta | 624h | **811h** | Onda 1 |

**Subtotal Cross:** 624h base → **811h** com margem

---

## 📊 RESUMO CONSOLIDADO (COM MARGEM 30%)

### Por Módulo

| Módulo | Qtd. Requisitos | Horas Base | Horas +30% |
|--------|-----------------|------------|------------|
| **Abertura** | 15 | 9.776h | **12.709h** |
| **Sinistro** | 31 | 18.512h | **24.066h** |
| **Assistência** | 16 | 9.984h | **12.979h** |
| **Financeiro** | 14 | 8.960h | **11.648h** |
| **Cross** | 1 | 624h | **811h** |
| **TOTAL** | **77** | **47.840h** | **62.192h** |

---

### Por Tipo de Requisito

| Tipo | Qtd. Requisitos | Horas Base | Horas +30% |
|------|-----------------|------------|------------|
| **Sistema** | 44 | 27.664h | **35.963h** |
| **Processo** | 29 | 17.472h | **22.714h** |
| **Aplicação** | 4 | 2.704h | **3.515h** |
| **TOTAL** | **77** | **47.840h** | **62.192h** |

---

### Por Porte

| Porte | Qtd. | Horas Unitárias Base | Horas Base Total | Horas +30% |
|-------|------|---------------------|------------------|------------|
| **P** (Pequeno) | 3 | 208h | 624h | **811h** |
| **M** (Médio) | 8 | 416h | 3.328h | **4.326h** |
| **G** (Grande) | 53 | 624h | 33.072h | **42.994h** |
| **GG** (Muito Grande) | 13 | 832h | 10.816h | **14.061h** |
| **TOTAL** | **77** | - | **47.840h** | **62.192h** |

---

### Por Complexidade

| Complexidade | Qtd. | Horas Base | Horas +30% |
|--------------|------|------------|------------|
| **Baixa** | 7 | 3.536h | **4.597h** |
| **Média** | 40 | 24.544h | **31.907h** |
| **Alta** | 30 | 19.760h | **25.688h** |
| **TOTAL** | **77** | **47.840h** | **62.192h** |

---

### Por Onda de Entrega

| Onda | Qtd. | Horas Base | Horas +30% | % do Total |
|------|------|------------|------------|------------|
| **Onda 1** | 25 | 14.352h | **18.658h** | 30% |
| **Onda 2** | 16 | 9.360h | **12.168h** | 20% |
| **Onda 3** | 23 | 16.016h | **20.821h** | 33% |
| **Time Autosserviço** | 8 | 4.992h | **6.490h** | 10% |
| **Despriorizado** | 5 | 3.120h | **4.056h** | 7% |
| **TOTAL** | **77** | **47.840h** | **62.192h** | 100% |

---

## ⏱️ ESTIMATIVA DE PRAZO (COM MARGEM 30%)

### Premissas
- Horas úteis por desenvolvedor/mês: **160h**
- Produtividade efetiva considerada: **100%** (margem já aplicada)

### Cenários de Equipe - PROJETO TOTAL (62.192 horas)

| Cenário | Desenvolvedores | Meses Totais | Anos | Prazo Recomendado |
|---------|-----------------|--------------|------|-------------------|
| **Conservador** | 5 | 77,7 meses | 6,5 anos | Não recomendado |
| **Moderado** | 10 | 38,9 meses | 3,2 anos | Longo prazo |
| **Recomendado** | 15 | 25,9 meses | **2,2 anos** | ✅ Equilibrado |
| **Agressivo** | 20 | 19,4 meses | 1,6 anos | Risco médio |
| **Muito Agressivo** | 25 | 15,5 meses | 1,3 anos | Alto risco |

---

### Por Onda (COM 15 DESENVOLVEDORES)

| Onda | Horas +30% | Meses Necessários | Prazo |
|------|------------|-------------------|-------|
| **Onda 1** | 18.658h | **7,8 meses** | ~8 meses |
| **Onda 2** | 12.168h | **5,1 meses** | ~5 meses |
| **Onda 3** | 20.821h | **8,7 meses** | ~9 meses |
| **Autosserviço** | 6.490h | Paralelo às ondas | - |
| **Despriorizado** | 4.056h | Backlog | - |
| **TOTAL ONDAS 1-3** | **51.647h** | **21,5 meses** | ~22 meses |

---

### Por Onda (COM 20 DESENVOLVEDORES)

| Onda | Horas +30% | Meses Necessários | Prazo |
|------|------------|-------------------|-------|
| **Onda 1** | 18.658h | **5,8 meses** | ~6 meses |
| **Onda 2** | 12.168h | **3,8 meses** | ~4 meses |
| **Onda 3** | 20.821h | **6,5 meses** | ~6-7 meses |
| **TOTAL ONDAS 1-3** | **51.647h** | **16,1 meses** | ~16-17 meses |

---

## 🔧 CONSIDERAÇÕES TÉCNICAS

### Stack Tecnológica e Impactos

| Tecnologia | Complexidade | Impacto na Estimativa |
|------------|--------------|----------------------|
| **Java 17+ / Spring Boot 3.x** | Média | Framework maduro, boa produtividade |
| **Oracle Database** | Alta | Requer DBAs especializados, procedures complexas |
| **Apache Kafka** | Alta | Eventos assíncronos, garantia de entrega, replay |
| **Sistemas Legados** | Muito Alta | SAP, GSA, ABAS, Cotador, Sibel - interfaces diversas |
| **Integrações Externas** | Alta | DETRAN, BCP, Bureau, WhatsApp Business API |

### Sistemas a Serem Integrados (Identificados na Planilha)

1. **SAP** - Sistema financeiro
2. **Cotador Auto Frota** - Emissão de apólices
3. **Nova Emissão R3** - Sistema de emissão
4. **GSA** - Gestão de Sinistros e Assistência
5. **ABAS** - Sistema de análise
6. **COL** - Portal do Corretor Online
7. **Portal da Produção** - Área comercial
8. **Portal do Cliente (PDC)** - Segurado
9. **Portal do Prestador** - Guinchos e oficinas
10. **LaudoWeb** - Laudos de vistoria
11. **Sibel** - Central de atendimento
12. **Terabox** - Comunicação com prestadores
13. **Sistema de Ticket** - Gestão de demandas
14. **WhatsApp Business API** - Chatbots
15. **Licitar** - Editais de licitação

### Riscos Identificados

| Risco | Probabilidade | Impacto | Mitigação |
|-------|---------------|---------|-----------|
| Integração com legados complexos | Alta | Alto | POCs antecipadas, API Gateway |
| Dependências entre módulos | Alta | Médio | Arquitetura Event-Driven com Kafka |
| Mudanças de escopo | Média | Alto | Sprints curtas, MVP por onda |
| Disponibilidade de DBAs Oracle | Média | Alto | Alocação dedicada desde o início |
| Conformidade regulatória (SUSEP) | Média | Alto | Envolver jurídico/compliance desde início |
| Performance em alto volume | Média | Médio | Testes de carga, cache distribuído |

---

## 📅 CRONOGRAMA SUGERIDO (20 Desenvolvedores)

```
┌────────────────────────────────────────────────────────────────────────────────────┐
│                         TIMELINE TOTAL - 17-18 MESES                               │
├────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                    │
│ M1-M2      │ ▓▓▓▓ Arquitetura Base, Infraestrutura, CI/CD, APIs Core               │
│                                                                                    │
│ M3-M8      │ ████████████████████████████████████████ ONDA 1 (6 meses)             │
│            │ • 25 requisitos                                                       │
│            │ • Foco: Processos estruturantes, treinamentos, bases                  │
│                                                                                    │
│ M9-M12     │ ████████████████████ ONDA 2 (4 meses)                                 │
│            │ • 16 requisitos                                                       │
│            │ • Foco: Automações, integrações, sistemas                             │
│                                                                                    │
│ M13-M18    │ ██████████████████████████████████████████ ONDA 3 (6 meses)           │
│            │ • 23 requisitos                                                       │
│            │ • Foco: Novos sistemas, IA, painéis, financeiro                       │
│                                                                                    │
│ PARALELO   │ ░░░░░░░░░░░░ Time Autosserviço (squad dedicado)                       │
│            │ • 8 requisitos - portais e autosserviço                               │
│                                                                                    │
└────────────────────────────────────────────────────────────────────────────────────┘
```

---

## 👥 ESTRUTURA DE EQUIPE RECOMENDADA (20 Desenvolvedores)

### Composição por Squad

| Squad | Foco | Desenvolvedores | Especialistas |
|-------|------|-----------------|---------------|
| **Squad Abertura** | Módulo de Abertura + Integrações | 4 devs | 1 Tech Lead |
| **Squad Sinistro** | Módulo de Sinistro + GSA/ABAS | 5 devs | 1 Tech Lead |
| **Squad Assistência** | Módulo de Assistência + Prestadores | 4 devs | 1 Tech Lead |
| **Squad Financeiro** | Módulo Financeiro + SAP | 4 devs | 1 Tech Lead |
| **Squad Autosserviço** | Portais + Apps + Bots | 3 devs | 1 Tech Lead |

### Papéis Adicionais Necessários

| Papel | Quantidade | Responsabilidade |
|-------|------------|------------------|
| **Arquiteto de Soluções** | 1 | Visão técnica, decisões de arquitetura |
| **DBA Oracle** | 2 | Modelagem, performance, procedures |
| **DevOps/SRE** | 2 | CI/CD, Kubernetes, monitoramento |
| **QA Lead** | 1 | Estratégia de testes, automação |
| **QA Analysts** | 4 | Testes funcionais, integração, UAT |
| **Product Owner** | 2 | Gestão de backlog, priorização |
| **Scrum Master** | 2 | Facilitação, métricas, impedimentos |
| **Tech Writer** | 1 | Documentação técnica e de usuário |

---

## 💰 ESTIMATIVA DE CUSTO (Referência)

### Premissas de Custo
- Custo médio desenvolvedor/hora: R$ 150,00 (mercado SP)
- Inclui encargos e overhead

| Cenário | Horas | Custo Estimado |
|---------|-------|----------------|
| **Base (sem margem)** | 47.840h | R$ 7.176.000 |
| **Com Margem 30%** | 62.192h | **R$ 9.328.800** |

> ⚠️ Valores de referência. Custos reais dependem de modelo de contratação, senioridade da equipe e localização.

---

## ✅ CHECKLIST DE VALIDAÇÃO

### Dados da Planilha Original Verificados

- [x] Total de requisitos: **77** ✓
- [x] Horas base totais: **47.840h** ✓
- [x] Distribuição por Tipo: Sistema (44), Processo (29), Aplicação (4) ✓
- [x] Distribuição por Porte: G (53), GG (13), M (8), P (3) ✓
- [x] Distribuição por Onda: Onda 1 (25), Onda 2 (16), Onda 3 (23), Autosserviço (8), Despriorizado (5) ✓
- [x] Distribuição por Complexidade: Alta (30), Média (40), Baixa (7) ✓
- [x] Margem de segurança aplicada: **+30%** ✓
- [x] Total final com margem: **62.192h** ✓

---

## 📌 RECOMENDAÇÕES FINAIS

1. **Iniciar pela Onda 1**: Requisitos estruturantes que habilitam as demais ondas
2. **Squad de Autosserviço em paralelo**: Não depende das outras ondas
3. **POCs de integração**: Iniciar POCs com SAP, GSA e Kafka no M1-M2
4. **Contratos de API**: Definir contratos antes do desenvolvimento
5. **Feature Flags**: Permitir releases graduais por cliente/região
6. **Observabilidade desde o início**: APM, logs, traces distribuídos
7. **Testes automatizados**: Mínimo 80% de cobertura de código crítico

---

*Documento gerado em: Dezembro/2024*
*Metodologia: SDLC + Story Points + Análise de Complexidade*
*Margem de Segurança: +30%*
*Fonte de Dados: Planilha "Porto Pós - Mapa de Resolução de Dores.xlsx"*
