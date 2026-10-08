# Guia de elaboração — PSI, PGR e PCN da AeroLog

## 1. Objetivo deste guia

Este documento define **como o grupo deverá estruturar e dividir a elaboração dos três documentos da atividade acadêmica**:

- **PSI — Política de Segurança da Informação**
- **PGR — Política/Plano de Gestão de Riscos**
- **PCN — Plano de Continuidade de Negócios**

A proposta é manter os três documentos **objetivos, complementares e coerentes entre si**, evitando repetição excessiva de conteúdo.

Os documentos devem ser elaborados **considerando como base principal o estudo de caso da AeroLog Transportes Aéreos fornecido na atividade**. As fontes externas indicadas neste guia devem ser usadas para orientar a estrutura, os conceitos e a forma de apresentação, mas o conteúdo deve ser adaptado ao cenário da AeroLog.

---

# 2. Caso de uso que deve orientar os três documentos

Todos os integrantes do grupo devem considerar, durante a elaboração, as características apresentadas no caso da **AeroLog Transportes Aéreos**.

## Características principais da empresa

- Empresa do ramo de logística aérea.
- Atua com transporte de cargas e passageiros.
- Possui aproximadamente **1.100 funcionários**.
- Atende cerca de **20 cidades brasileiras**.
- Mantém aproximadamente **50 servidores locais**.
- Possui **sistemas críticos embarcados em aeronaves**.
- Possui equipe própria de TI.
- Mantém **contratos internacionais de suporte com fornecedores de software de navegação**.
- O último treinamento em cibersegurança ocorreu há aproximadamente **quatro anos**.
- Os equipamentos são renovados, em média, a cada **cinco anos**.
- Os sistemas de controle e reservas já são alvo de:
  - ataques de negação de serviço (DDoS);
  - tentativas de fraude de passagens.

## Pontos específicos exigidos pelo estudo de caso

### Para a PSI

A política deve considerar principalmente:

- proteção dos sistemas de reservas;
- proteção dos dados dos passageiros;
- LGPD;
- requisitos e regulamentações de cibersegurança aplicáveis ao setor aéreo;
- proteção dos sistemas embarcados;
- controle do acesso de fornecedores externos;
- segurança do acesso remoto;
- conscientização e treinamento dos colaboradores.

### Para a PGR

Devem ser considerados, no mínimo, os seguintes riscos apresentados no caso:

- fraude na emissão de passagens;
- ataques DDoS contra o sistema de reservas;
- comprometimento de sistemas por meio de fornecedores externos;
- falhas em sistemas legados;
- comprometimento de sistemas críticos ou embarcados.

Outros riscos podem ser acrescentados se forem coerentes com o cenário.

### Para o PCN

O plano deve abordar principalmente:

- continuidade do sistema de reservas;
- utilização de backups e mecanismos de recuperação;
- continuidade das operações de voo durante indisponibilidades;
- isolamento de sistemas embarcados em caso de comprometimento;
- comunicação e acionamento das áreas e autoridades necessárias;
- retomada segura dos serviços críticos.

---

# 3. Relação entre PSI, PGR e PCN

Os documentos devem ser tratados como partes de uma mesma estratégia.

## PSI — define as regras

A PSI estabelece **o que a AeroLog deve proteger e quais princípios e diretrizes de segurança devem ser seguidos**.

Exemplo:

> A AeroLog deve adotar medidas destinadas a assegurar a disponibilidade dos sistemas críticos e manter procedimentos de continuidade e recuperação.

A PSI não precisa explicar detalhadamente como recuperar cada sistema.

---

## PGR — identifica e trata os riscos

A PGR identifica **o que pode dar errado**, avalia a gravidade desses riscos e determina como eles serão tratados.

Exemplo:

> R01 — Ataque DDoS ao sistema de reservas.  
> Probabilidade: alta.  
> Impacto: alto.  
> Tratamento: mitigação por meio de proteção contra DDoS, redundância e monitoramento.

Quando um risco puder causar paralisação das operações, a PGR pode fazer referência ao PCN.

---

## PCN — determina como continuar ou recuperar a operação

O PCN explica **o que deve ser feito quando um incidente realmente causar indisponibilidade ou interrupção relevante**.

Exemplo:

> C01 — Indisponibilidade do sistema de reservas.  
> Riscos relacionados: R01 — DDoS e R04 — falha de infraestrutura.  
> Ações: ativar o ambiente de contingência, verificar a integridade dos dados, restaurar o serviço e comunicar as áreas responsáveis.

---

## Fluxo entre os documentos

```text
PSI
│
│ Define princípios, regras e obrigações de segurança.
│
▼
PGR
│
│ Identifica, avalia e trata os riscos que podem
│ afetar os ativos e processos protegidos pela PSI.
│
▼
PCN
│
│ Define o que fazer quando determinados riscos
│ causarem interrupção das operações.
│
▼
Retomada das operações
```

A ideia é evitar três documentos independentes tratando das mesmas coisas.

---

# 4. Estrutura objetiva da PSI

## Finalidade da PSI

A PSI deve responder principalmente:

> **Quais são as regras, princípios e diretrizes de segurança da informação que a AeroLog deve seguir?**

O documento deve permanecer em nível de **política**, sem transformar cada diretriz em um procedimento técnico detalhado.

## Estrutura recomendada

### 1. Objetivo

Explicar de forma breve o propósito da PSI.

Deve mencionar a proteção:

- das informações;
- dos sistemas;
- dos dados dos passageiros;
- dos serviços críticos;
- dos sistemas de reservas e operações aéreas.

### 2. Escopo

Definir a quem e ao que a política se aplica.

Considerar:

- funcionários;
- equipe de TI;
- pilotos e engenheiros;
- prestadores de serviço;
- fornecedores nacionais e internacionais;
- servidores;
- sistemas de reservas;
- sistemas embarcados;
- dados pessoais;
- demais ativos de informação.

### 3. Princípios de Segurança da Informação

Apresentar de forma objetiva princípios como:

- confidencialidade;
- integridade;
- disponibilidade;
- autenticidade;
- menor privilégio;
- necessidade de acesso;
- proteção de dados pessoais.

### 4. Diretrizes de Segurança

Este deve ser o principal tópico da PSI.

Pode ser dividido em subtópicos curtos:

#### 4.1 Controle de acesso

- acessos individuais;
- menor privilégio;
- revisão de permissões;
- proteção de contas privilegiadas.

#### 4.2 Sistemas de reservas e dados de passageiros

- proteção contra acesso não autorizado;
- prevenção de fraude;
- proteção de dados pessoais;
- monitoramento.

#### 4.3 Sistemas críticos e embarcados

- restrição de acesso;
- atualizações controladas;
- proteção contra alterações não autorizadas;
- segregação quando aplicável.

#### 4.4 Fornecedores e acesso remoto

- autorização formal;
- acesso somente quando necessário;
- registro e monitoramento;
- requisitos de segurança em contratos.

#### 4.5 Vulnerabilidades e atualizações

- atualizações periódicas;
- avaliação de sistemas legados;
- correções de segurança.

#### 4.6 Backup e recuperação

- realização periódica de backups;
- proteção das cópias;
- testes de restauração;
- existência de cópias adequadas para contingência.

#### 4.7 Incidentes de segurança

- obrigação de comunicar incidentes;
- registro;
- tratamento;
- acionamento das áreas responsáveis.

#### 4.8 Treinamento e conscientização

Este item é especialmente relevante porque o caso informa que o último treinamento ocorreu há quatro anos.

Prever:

- treinamento periódico;
- conscientização contra phishing e fraude;
- treinamento adequado à função de cada colaborador.

### 5. Papéis e Responsabilidades

Manter este tópico simples.

Separar, por exemplo:

- Alta Administração;
- TI/Segurança da Informação;
- gestores;
- colaboradores;
- fornecedores e terceiros.

### 6. Conformidade, Revisão e Atualização

Informar que:

- a política deve observar legislação e regulamentação aplicáveis;
- deve ser revisada periodicamente;
- mudanças relevantes no ambiente tecnológico ou regulatório podem motivar revisão antecipada.

---

# 5. Estrutura objetiva da PGR

## Finalidade da PGR

A PGR deve responder:

> **Quais são os principais riscos da AeroLog, qual a gravidade de cada um e como devem ser tratados?**

Como a atividade pede identificação, avaliação e mitigação, a PGR deve possuir uma parte metodológica pequena e uma parte prática maior.

## Estrutura recomendada

### 1. Objetivo e Escopo

Explicar:

- por que a gestão de riscos será realizada;
- quais sistemas, processos e ativos estão incluídos.

Priorizar:

- sistema de reservas;
- sistemas de voo;
- infraestrutura de TI;
- sistemas embarcados;
- fornecedores externos;
- dados dos passageiros.

### 2. Metodologia de Avaliação

Explicar de maneira simples como os riscos serão avaliados.

Sugestão:

#### Probabilidade

- Baixa
- Média
- Alta

#### Impacto

- Baixo
- Médio
- Alto
- Crítico

#### Nível de risco

Definir uma matriz simples relacionando probabilidade e impacto.

Não é necessário criar uma metodologia complexa para a atividade.

### 3. Identificação e Avaliação dos Riscos

Este deve ser o principal tópico do documento.

Sugestão de tabela:

| ID | Risco | Ativo/Processo afetado | Probabilidade | Impacto | Nível |
|---|---|---|---|---|---|
| R01 | DDoS contra o sistema de reservas | Reservas | Alta | Alto | Crítico |
| R02 | Fraude na emissão de passagens | Reservas/GDS | Alta | Alto | Crítico |
| R03 | Comprometimento por fornecedor externo | Sistemas críticos | Média | Alto | Alto |
| R04 | Falha de sistema legado | Operações/TI | Média | Alto | Alto |
| R05 | Comprometimento de sistema embarcado | Operações de voo | Baixa | Crítico | Alto |

Os valores acima são apenas uma proposta inicial e podem ser ajustados pelo grupo, desde que justificados.

### 4. Tratamento dos Riscos

Utilizar os mesmos IDs criados anteriormente.

Sugestão:

| ID | Estratégia | Medidas propostas |
|---|---|---|
| R01 | Mitigar | Proteção anti-DDoS, monitoramento e redundância |
| R02 | Mitigar | Monitoramento antifraude, controles de acesso e registros |
| R03 | Mitigar | Controle de acesso remoto, MFA, registro de sessões e requisitos contratuais |
| R04 | Mitigar | Atualização, substituição planejada, redundância e monitoramento |
| R05 | Mitigar | Isolamento, controle de alterações e restrição de acesso |

Quando o risco também exigir continuidade de negócios, indicar o cenário correspondente do PCN.

Exemplo:

> R01 — consultar também PCN/C01 — Indisponibilidade do sistema de reservas.

### 5. Responsabilidades

Definir de maneira breve:

- quem acompanha os riscos;
- quem aprova os tratamentos;
- quem executa as medidas;
- quem comunica alterações relevantes.

### 6. Monitoramento e Revisão

Definir que:

- riscos devem ser revistos periodicamente;
- novos incidentes podem gerar novos riscos;
- mudanças em sistemas, fornecedores ou operações podem exigir reavaliação.

---

# 6. Estrutura objetiva do PCN

## Finalidade do PCN

O PCN deve responder:

> **Como a AeroLog continuará operando ou retomará suas operações quando ocorrer uma interrupção grave?**

Ele deve ser mais operacional que a PSI e a PGR.

## Estrutura recomendada

### 1. Objetivo e Escopo

Definir:

- finalidade do plano;
- processos abrangidos;
- tipos de interrupção que podem levar à sua ativação.

### 2. Processos e Sistemas Críticos

Identificar os serviços que devem receber prioridade.

Sugestão:

| Processo/Sistema | Criticidade | Prioridade de recuperação |
|---|---|---|
| Operações de voo | Crítica | 1 |
| Sistemas embarcados críticos | Crítica | 1 |
| Sistema de reservas | Crítica | 2 |
| Check-in/embarque | Crítica | 2 |
| Sistemas administrativos | Média | 3 |

### 3. Impactos e Prioridades de Recuperação

Explicar brevemente:

- o que acontece se cada processo ficar indisponível;
- quais processos precisam retornar primeiro;
- dependências importantes.

Se o grupo desejar utilizar **RTO e RPO**, os valores devem ser apresentados como **premissas definidas para a atividade**, pois o estudo de caso não fornece esses tempos.

### 4. Estratégias de Continuidade

Apresentar medidas gerais, como:

- redundância;
- utilização de backups;
- cópias offline quando aplicável;
- procedimentos manuais ou alternativos;
- isolamento de sistemas comprometidos;
- infraestrutura alternativa;
- canais alternativos de comunicação.

### 5. Cenários de Contingência, Resposta e Recuperação

Este deve ser o principal tópico do PCN.

Criar poucos cenários, mas diretamente relacionados ao caso.

#### C01 — Indisponibilidade do sistema de reservas

Riscos relacionados:

- R01 — DDoS;
- R04 — falha de sistema.

Abordar:

- identificação da indisponibilidade;
- acionamento dos responsáveis;
- ativação da contingência;
- recuperação;
- validação;
- retorno à operação normal.

#### C02 — Comprometimento de sistema crítico ou embarcado

Risco relacionado:

- R05.

Abordar:

- isolamento;
- restrição de acesso;
- acionamento das equipes técnicas;
- avaliação da integridade;
- restauração ou substituição segura;
- comunicação conforme necessidade.

#### C03 — Comprometimento por fornecedor externo

Risco relacionado:

- R03.

Abordar:

- suspensão ou revogação temporária do acesso;
- análise dos registros;
- isolamento dos sistemas afetados;
- recuperação;
- revisão das credenciais e acessos.

#### C04 — Incidente cibernético de grande impacto

Pode incluir:

- ransomware;
- invasão;
- comprometimento simultâneo de servidores;
- indisponibilidade prolongada.

Abordar:

- isolamento;
- acionamento da equipe responsável;
- utilização dos backups;
- recuperação por prioridade;
- preservação de evidências;
- comunicação.

### 6. Comunicação

Definir, de maneira objetiva:

- comunicação interna;
- comunicação com passageiros, se necessária;
- contato com fornecedores;
- comunicação com autoridades e órgãos reguladores quando aplicável.

Considerar especialmente **ANAC e DECEA**, conforme indicado no estudo de caso.

### 7. Papéis e Responsabilidades

Definir responsáveis por:

- ativação do PCN;
- decisão operacional;
- recuperação técnica;
- comunicação;
- retorno à normalidade.

### 8. Testes e Revisão

Prever:

- testes periódicos;
- simulações;
- revisão após incidentes;
- atualização quando houver mudanças relevantes.

---

# 7. Divisão recomendada para o trabalho em grupo

Os três documentos podem ser desenvolvidos por pessoas diferentes, mas devem utilizar os mesmos conceitos e nomenclaturas.

## Pessoa ou subgrupo responsável pela PSI

Deve concentrar-se em:

- princípios;
- regras;
- diretrizes;
- responsabilidades;
- segurança dos ativos.

Não deve detalhar excessivamente riscos individuais nem procedimentos de recuperação.

---

## Pessoa ou subgrupo responsável pela PGR

Deve concentrar-se em:

- identificação;
- probabilidade;
- impacto;
- classificação;
- tratamento dos riscos.

Deve criar e manter os IDs de risco, por exemplo:

- R01
- R02
- R03

Esses IDs poderão ser utilizados pelo PCN.

---

## Pessoa ou subgrupo responsável pelo PCN

Deve concentrar-se em:

- interrupções;
- processos críticos;
- prioridade;
- contingência;
- recuperação;
- comunicação.

Deve relacionar os cenários aos riscos definidos na PGR.

Exemplo:

- C01 relacionado a R01 e R04;
- C02 relacionado a R05.

---

## Revisão final conjunta

Antes da entrega, o grupo deve verificar se:

1. todos utilizaram os mesmos nomes para sistemas e processos;
2. os riscos citados no PCN realmente existem na PGR;
3. as diretrizes da PSI são compatíveis com os tratamentos propostos na PGR;
4. não existem contradições entre os documentos;
5. os documentos permanecem objetivos;
6. todas as informações apresentadas como fatos sobre a AeroLog estão presentes no estudo de caso;
7. hipóteses criadas pelo grupo estão claramente identificadas como propostas ou premissas acadêmicas.

---

# 8. Fontes externas que serão utilizadas

As fontes externas devem ser usadas principalmente para **estrutura, conceitos, linguagem e exemplos de controles**.

Não devem substituir o estudo de caso.

A prioridade sugerida é:

1. documentos oficiais brasileiros;
2. materiais da ANAC para particularidades do setor aéreo;
3. documentos públicos de companhias aéreas como referência prática;
4. outras normas ou referências somente se forem realmente necessárias.

---

## 8.1 PSI — Modelo de Política de Segurança da Informação do PPSI 2.0

**Fonte:** Governo Digital / Ministério da Gestão e da Inovação em Serviços Públicos.

**Página oficial do PPSI 2.0:**

https://www.gov.br/governodigital/pt-br/privacidade-e-seguranca/ppsi-2.0

**Página com os arquivos e modelos:**

https://www.gov.br/governodigital/pt-br/privacidade-e-seguranca/ppsi-2.0/arquivos

### Como utilizar

O modelo deve servir como **principal referência estrutural para a PSI**.

Observar principalmente como o documento organiza:

- finalidade;
- escopo;
- princípios;
- diretrizes;
- responsabilidades;
- revisão;
- disposições finais.

Não copiar integralmente os artigos ou referências destinadas à Administração Pública.

A AeroLog é uma empresa privada fictícia, portanto termos como:

- órgão;
- agente público;
- autoridade administrativa;
- SISP;

devem ser substituídos por uma redação compatível com a empresa.

O grupo já possui uma cópia do **Modelo de Política de Segurança da Informação — PPSI 2.0**, que pode ser consultada durante a elaboração.

---

## 8.2 PGR — Kit de Gestão de Riscos de Segurança da Informação

**Fonte:** Ministério da Gestão e da Inovação em Serviços Públicos.

**Link:**

https://www.gov.br/gestao/pt-br/assuntos/estatais/central-de-conteudo/kits-governanca-ti/kit-2/gestao-de-riscos-de-seguranca-da-informacao

### Como utilizar

Esta fonte possui materiais específicos para gestão de riscos, incluindo:

- artefato de gestão de riscos;
- passo a passo;
- formulário de categorias e parâmetros;
- template de Plano de Gestão de Riscos de Segurança da Informação;
- template de Plano de Tratamento de Riscos.

Para esta atividade, utilizar principalmente como referência para:

- identificação dos riscos;
- definição de probabilidade;
- definição de impacto;
- classificação;
- tratamento;
- acompanhamento.

Não é necessário reproduzir toda a complexidade dos modelos oficiais.

O objetivo é aproveitar a lógica da metodologia e produzir uma PGR curta e adequada ao caso da AeroLog.

---

## 8.3 PCN — Plano de Continuidade de Negócios do MGI

**Fonte:** Ministério da Gestão e da Inovação em Serviços Públicos.

**Link direto para o documento:**

https://www.gov.br/gestao/pt-br/acesso-a-informacao/acoes-e-programas/programas-projetos-acoes-obras-e-atividades/copy_of_PlanodeContinuidadedeNegcios_v1.1.pdf

### Como utilizar

Utilizar como referência para observar como um PCN real organiza:

- governança;
- processos críticos;
- análise de impacto;
- estratégias de continuidade;
- responsabilidades;
- recuperação;
- testes e manutenção.

Para a atividade, utilizar apenas os elementos necessários.

Não tentar reproduzir a extensão ou o nível de detalhamento do documento governamental.

---

## 8.4 PCN — Modelos de Gestão de Continuidade da SEFAZ-DF

**Fonte:** Secretaria de Estado de Fazenda do Distrito Federal.

**Link:**

https://static.fazenda.df.gov.br/arquivos/pdf/PCN/022014/modelos___gestao_de_continuidade_de_negocios_e_de_ti_da_sefaz_df_docx.pdf

### Como utilizar

Esta fonte é útil principalmente para entender a parte prática de:

- análise de impacto nos negócios;
- levantamento de recursos;
- identificação de dependências;
- criticidade;
- tempo máximo de interrupção;
- estratégias de contingência.

Pode ser usada como apoio na construção das tabelas do PCN.

Por ser um material mais antigo, deve ser considerado principalmente como **referência de estrutura e formulários**, e não como única fonte normativa.

---

# 9. Fontes específicas do setor aéreo

## 9.1 ANAC — Segurança Cibernética na Aviação Civil

**Fonte:** Agência Nacional de Aviação Civil.

**Link:**

https://www.gov.br/anac/pt-br/assuntos/seguranca-cibernetica-na-aviacao-civil

### Como utilizar

Esta deve ser uma das principais referências para contextualizar os documentos no setor aéreo.

Pode auxiliar especialmente na justificativa de medidas relacionadas a:

- sistemas críticos;
- riscos cibernéticos;
- resiliência;
- proteção da infraestrutura;
- resposta a incidentes;
- conscientização;
- segurança das operações.

A fonte deve ser utilizada para tornar PSI, PGR e PCN coerentes com o contexto de uma empresa de aviação, sem perder o foco no estudo de caso.

---

## 9.2 ANAC — Gestão de Continuidade de Serviços de TI

**Fonte:** Portaria nº 9.459/STI, de 6 de outubro de 2022.

**Link:**

https://www.anac.gov.br/assuntos/legislacao/legislacao-1/portarias/2022/portaria-9459

### Como utilizar

Usar principalmente como apoio para o PCN.

Observar conceitos relacionados a:

- análise de impacto;
- atividade crítica;
- ativos críticos;
- prioridade de recuperação;
- continuidade de serviços de TI.

O documento é da própria ANAC e, portanto, é especialmente útil para compreender como continuidade e criticidade são tratadas dentro do contexto da aviação civil.

---

# 10. Referência prática de companhia aérea

## GOL — Política de Segurança da Informação para Terceiros

**Fonte:** GOL Linhas Aéreas.

**Link direto para o PDF:**

https://static.voegol.com.br/voegol/2025-06-27/PO-DTI-SC-003-Pol%C3%ADtica%20de%20Seguran%C3%A7a%20da%20Informa%C3%A7%C3%A3o%20para%20Terceiro_r01.pdf

**Página de fornecedores da GOL:**

https://www.voegol.com.br/sobre-a-gol/fornecedores

### Como utilizar

Este documento não deve ser usado como modelo principal da PSI, porque seu escopo é especificamente a relação da GOL com terceiros.

Entretanto, é uma referência prática muito útil para o caso da AeroLog, principalmente porque a empresa fictícia possui **fornecedores internacionais com acesso ou suporte a sistemas importantes**.

Observar especialmente como uma companhia aérea real trata:

- confidencialidade, integridade e disponibilidade;
- requisitos para terceiros;
- acesso a informações;
- proteção de ativos;
- obrigações de fornecedores;
- continuidade e recuperação;
- requisitos contratuais de segurança.

As ideias podem ser adaptadas para a seção de **fornecedores e acesso remoto da PSI** e para riscos de terceiros na **PGR**.

Não copiar controles internos da GOL como se fossem requisitos obrigatórios da AeroLog.

---

# 11. Como as fontes devem ser usadas

## Fonte principal do conteúdo

O **estudo de caso da AeroLog** é a fonte principal para determinar:

- contexto;
- tamanho;
- infraestrutura;
- ameaças;
- fragilidades;
- necessidades;
- prioridades.

Não devem ser inventados fatos adicionais sobre a AeroLog sem deixar claro que se trata de uma premissa adotada pelo grupo.

---

## Fontes governamentais

Utilizar Gov.br, MGI, ANAC e SEFAZ-DF principalmente para:

- estruturar os documentos;
- usar terminologia adequada;
- compreender os componentes esperados;
- fundamentar os conceitos;
- criar tabelas e métodos simplificados.

---

## Documentos de companhias aéreas

Utilizar como **referência prática e setorial**, especialmente para observar como uma empresa aérea real redige políticas e trata temas semelhantes.

Não utilizar como única fonte metodológica.

---

# 12. Critério de objetividade

A atividade não exige que os documentos possuam o mesmo nível de detalhamento de documentos corporativos reais.

Por isso, o grupo deve priorizar:

- frases curtas e claras;
- poucos tópicos;
- tabelas para riscos, processos críticos e responsabilidades;
- controles diretamente relacionados ao caso;
- referências cruzadas entre PSI, PGR e PCN;
- justificativas breves.

Evitar:

- longas introduções teóricas;
- copiar leis inteiras;
- repetir o mesmo controle nos três documentos;
- criar dezenas de riscos pouco relevantes;
- detalhar procedimentos técnicos que não foram solicitados;
- criar números, métricas ou características da AeroLog sem indicar que são premissas.

---

# 13. Resumo da estrutura final

## PSI

1. Objetivo
2. Escopo
3. Princípios de Segurança da Informação
4. Diretrizes de Segurança
5. Papéis e Responsabilidades
6. Conformidade, Revisão e Atualização

---

## PGR

1. Objetivo e Escopo
2. Metodologia de Avaliação
3. Identificação e Avaliação dos Riscos
4. Tratamento dos Riscos
5. Responsabilidades
6. Monitoramento e Revisão

---

## PCN

1. Objetivo e Escopo
2. Processos e Sistemas Críticos
3. Impactos e Prioridades de Recuperação
4. Estratégias de Continuidade
5. Cenários de Contingência, Resposta e Recuperação
6. Comunicação
7. Papéis e Responsabilidades
8. Testes e Revisão

---

# 14. Regra geral para o grupo

Durante a elaboração, utilizar a seguinte lógica:

> **PSI:** o que deve ser protegido e quais regras devem ser seguidas.

> **PGR:** quais riscos ameaçam aquilo que a PSI protege e como serão tratados.

> **PCN:** o que fazer quando um desses riscos provocar uma interrupção relevante.

Sempre que houver dúvida sobre incluir determinado conteúdo em um dos três documentos, usar essas três perguntas para decidir onde ele pertence.

O resultado final deve demonstrar que **PSI, PGR e PCN são documentos diferentes, mas fazem parte de uma mesma estratégia de segurança, gestão de riscos e continuidade da AeroLog Transportes Aéreos**.
