# 📋 GUIA OPERACIONAL - TeepOEE Duplo Palete
## Sistema de Monitoramento OEE para Máquinas com Duplo Palete

---

## 🎯 **OBJETIVO DO PRODUTO**

O **TeepOEE - Duplo Palete** é um sistema avançado de monitoramento e controle de eficiência operacional desenvolvido especificamente para máquinas industriais com sistema de duplo palete. Este produto foi criado para atender às necessidades críticas da indústria moderna de manufatura, oferecendo:

- **Monitoramento em tempo real** de máquinas com duplo palete, permitindo acompanhamento contínuo do status operacional, posicionamento dos paletes e estados de produção
- **Cálculo automático de OEE** (Overall Equipment Effectiveness), fornecendo métricas precisas de disponibilidade, performance e qualidade para análise de eficiência
- **Controle de produção** por ordem de produção (OP), garantindo rastreabilidade completa desde o planejamento até a execução
- **Gestão de operadores** e turnos de trabalho, com controle de acesso, registro de responsabilidades e análise de performance por operador
- **Análise de paradas** e identificação de gargalos, oferecendo insights detalhados sobre causas de ineficiência e oportunidades de melhoria

**Contexto Industrial**: Em ambientes de produção com duplo palete, a eficiência depende diretamente da coordenação perfeita entre os dois paletes, otimização de tempos de setup e minimização de paradas não programadas. O TeepOEE foi desenvolvido para resolver exatamente esses desafios operacionais.

---

## 🔧 **CONCEITOS OPERACIONAIS FUNDAMENTAIS**

### **1. Sistema de Duplo Palete**

**Conceito**: O sistema de duplo palete é uma tecnologia avançada que permite máxima eficiência operacional através da alternância inteligente entre dois paletes. Enquanto um palete está em produção, o outro pode ser preparado com a próxima ordem, eliminando tempos mortos.

**Funcionamento**:
- **Palete 1 (P1)** e **Palete 2 (P2)** alternam na máquina de forma coordenada
- Apenas **um palete por vez** pode estar em produção ativa, garantindo segurança operacional
- **Troca automática** entre paletes é executada pelo sistema para maximizar eficiência e minimizar tempos de setup
- **Sensores físicos** detectam presença, posição e estado de cada palete em tempo real
- **Sistema de controle** gerencia toda a alternância automática, coordenando movimentos e transições

**Benefícios**: Redução de 40-60% no tempo total de produção, eliminação de tempos mortos entre ordens e aumento significativo da capacidade produtiva.

### **2. Ordem de Produção (OP)**

**Conceito**: A Ordem de Produção é o documento central que define toda a execução de uma tarefa de manufatura, contendo todas as informações necessárias para produção eficiente e rastreabilidade completa.

**Componentes**:
- **Código único** para cada ordem de produção, garantindo identificação única no sistema
- **Quantidade planejada** definida pelo planejamento de produção baseado em demandas e capacidade
- **Tempo de ciclo** específico para cada produto, calculado com base em estudos de tempo e métodos
- **Operador responsável** pela execução, garantindo accountability e controle de qualidade
- **Status de execução** (Aberta, Em Produção, Concluída, Cancelada) para controle de progresso

**Contexto**: Cada OP representa um compromisso de produção com cliente interno ou externo, sendo fundamental para o cumprimento de prazos e qualidade.

### **3. Estados Operacionais da Máquina**

**Conceito**: O sistema monitora continuamente o estado operacional da máquina, classificando cada momento em categorias específicas para análise precisa de eficiência.

**Estados Principais**:
- **🟡 SETUP**: Preparação da máquina para nova produção, incluindo troca de ferramentas, ajustes e configurações específicas do produto
- **🟢 PRODUÇÃO**: Máquina executando peças ativamente, com todos os sistemas funcionando dentro dos parâmetros operacionais
- **🔴 PARADA**: Máquina parada por anomalia, manutenção programada ou emergência, requerendo intervenção técnica
- **⚫ AGUARDANDO**: Esperando próxima ordem, operador ou condições específicas para retomada da operação

**Importância**: A classificação correta dos estados é fundamental para cálculo preciso do OEE e identificação de oportunidades de melhoria.

---

## 📊 **FLUXO OPERACIONAL PASSO A PASSO**

### **CENÁRIO 1: Início de Produção (Máquina Vazia)**

**Contexto**: Este cenário representa o início de um turno de trabalho ou a retomada de operações após parada prolongada. É fundamental estabelecer corretamente todas as condições operacionais para garantir eficiência durante todo o turno.

1. **Registrar Operador da Máquina**
   - **Acessar sistema TeepOEE** através da interface operacional
   - **Selecionar máquina de duplo palete** específica do chão de fábrica
   - **Registrar operador responsável pelo turno** com credenciais válidas
   - **Confirmar login do operador** para ativação do sistema de monitoramento
   
   **Importância**: O registro correto do operador é essencial para accountability, análise de performance individual e cumprimento de procedimentos de segurança.

2. **Abrir Primeira Ordem de Produção**
   - **Selecionar OP do sistema de planejamento** baseado em prioridades e disponibilidade de materiais
   - **Associar OP ao palete disponível** (P1 ou P2) conforme estratégia operacional
   - **Confirmar abertura da ordem** após validação de todos os parâmetros
   - **Resultado**: Palete entra automaticamente na máquina em **SETUP**, iniciando processo de preparação
   
   **Contexto**: A seleção da primeira OP influencia toda a sequência de produção do turno, sendo importante considerar tempos de setup e eficiência operacional.

3. **Iniciar Produção**
   - **Operador confirma setup completo** após verificação de todos os parâmetros (ferramentas, materiais, configurações)
   - **Sistema registra início de produção** com timestamp preciso para cálculo de OEE
   - **Resultado**: Transição **SETUP → PRODUÇÃO** com ativação de todos os contadores automáticos
   - **Contadores automáticos iniciam contagem** de peças, tempo de ciclo e métricas de qualidade
   
   **Benefícios**: Esta transição marca o início da produção efetiva, com todos os sistemas de monitoramento ativos para análise contínua de performance.

### **CENÁRIO 2: Segunda OP (Máquina Ocupada)**

**Contexto**: Este cenário demonstra a principal vantagem do sistema de duplo palete - a capacidade de preparar a próxima ordem enquanto a atual está em produção, maximizando eficiência operacional e minimizando tempos mortos.

1. **Abrir Segunda Ordem de Produção**
   - **Selecionar nova OP do planejamento** considerando sequência otimizada de produção
   - **Associar ao palete disponível** (diferente do ativo) para preparação paralela
   - **Confirmar abertura da ordem** após validação de materiais e ferramentas necessárias
   - **Resultado**: Palete fica **fora da máquina** aguardando momento ideal para troca
   
   **Estratégia**: A seleção da segunda OP deve considerar tempos de setup, similaridade de produtos e eficiência de troca para otimizar o fluxo produtivo.

2. **Troca Automática de Paletes**
   - **Sistema detecta OP pronta no segundo palete** através de sensores e validações automáticas
   - **Troca automática é executada** no momento mais eficiente (final de ciclo ou parada programada)
   - **Resultado**: 
     - Palete atual sai da máquina após conclusão da produção ou setup da próxima OP
     - Palete com nova OP entra em **SETUP** com todas as configurações necessárias
     - Produção para no palete anterior para permitir troca segura
   
   **Benefícios**: Esta troca automática elimina tempos mortos entre ordens, aumentando significativamente a eficiência operacional.

3. **Continuar Produção**
   - **Operador confirma setup da nova OP** após verificação completa de todos os parâmetros
   - **Sistema registra início de produção** com continuidade dos contadores de OEE
   - **Resultado**: Nova OP inicia produção automaticamente com transição suave
   
   **Impacto**: Esta continuidade garante que o OEE seja calculado de forma contínua, refletindo a eficiência real do sistema de duplo palete.

### **CENÁRIO 3: Parada por Anomalia**

**Contexto**: Paradas por anomalia são eventos críticos que impactam diretamente o OEE e a eficiência operacional. O registro adequado dessas paradas é fundamental para análise de causas raiz e implementação de melhorias preventivas.

1. **Registrar Parada**
   - **Operador identifica anomalia na máquina** através de indicadores visuais, sonoros ou sensores
   - **Acessa sistema TeepOEE** imediatamente para registro preciso do evento
   - **Seleciona "Registrar Parada"** na interface operacional
   - **Timer de segurança inicia (10 segundos)** para garantir que o operador tenha tempo de avaliar a situação
   
   **Importância**: O registro imediato é crucial para análise precisa do impacto no OEE e para identificação de padrões de falhas.

2. **Classificar Parada**
   - **Motivo da parada (obrigatório)** selecionado de lista padronizada para consistência na análise
   - **Descrição detalhada da anomalia** incluindo sintomas observados e condições operacionais
   - **Severidade (Alta/Média/Baixa)** baseada em impacto na produção e segurança
   - **Operador (registrado automaticamente)** para accountability e análise de performance
   - **Confirmar registro da parada** para ativação do cronômetro de parada
   
   **Benefícios**: Esta classificação padronizada permite análise estatística de paradas, identificação de causas mais frequentes e desenvolvimento de ações preventivas.

3. **Retomar Produção**
   - **Após correção da anomalia** e validação de que a máquina está operacional
   - **Operador confirma retomada** através da interface do sistema
   - **Sistema registra fim da parada** com timestamp preciso
   - **Máquina volta ao estado anterior** (SETUP ou PRODUÇÃO) conforme apropriado
   - **Tempo de parada é contabilizado no OEE** para cálculo preciso de disponibilidade
   
   **Impacto**: O registro correto do tempo de parada é essencial para cálculo preciso do OEE e para análise de eficiência operacional real.

---

## 🎛️ **INTERFACE OPERACIONAL**

### **Funcionalidades Principais**

**Gestão de OPs**: Sistema completo de controle de ordens de produção, incluindo abertura baseada em planejamento, monitoramento de progresso em tempo real, controle de quantidades produzidas vs. planejadas, e fechamento com registro de motivos e resultados finais.

**Monitoramento de Produção**: Controle contínuo em tempo real de todos os aspectos da produção, incluindo status da máquina, posicionamento dos paletes, contadores de peças, tempos de ciclo e indicadores de qualidade.

**Troca de Paletes**: Gerenciamento automático e inteligente do sistema de duplo palete, coordenando movimentos, validações de segurança e otimização de tempos de transição para máxima eficiência operacional.

**Registro de Paradas**: Sistema robusto de classificação e análise de anomalias, incluindo categorização por tipo, severidade e impacto, com geração automática de relatórios para análise de causas raiz.

**Controle de Operadores**: Gestão completa de turnos e responsabilidades, incluindo login/logout, controle de acesso, registro de atividades e análise de performance individual por operador.

**Relatórios OEE**: Análise detalhada de eficiência operacional com métricas de disponibilidade, performance e qualidade, incluindo tendências históricas e comparações entre turnos.

### **Indicadores Visuais**

**Status da Máquina**: Sistema de cores intuitivo que indica estado operacional atual (🟡 Setup, 🟢 Produção, 🔴 Parada, ⚫ Aguardando), permitindo identificação rápida de situações que requerem atenção.

**Indicadores de Paletes**: Display visual claro mostrando estado de cada palete (ativo, aguardando, com OP associada) e código da OP correspondente, facilitando controle operacional.

**Sinais Digitais**: Representação em tempo real dos sensores físicos da máquina, incluindo presença de paletes, posição na máquina e status de execução, fornecendo feedback visual imediato.

**Barra de Progresso**: Indicador visual do avanço da OP ativa, mostrando percentual concluído, quantidade produzida vs. planejada e tempo estimado para conclusão.

**Métricas OEE**: Display em tempo real das métricas de eficiência (Disponibilidade, Performance, Qualidade e OEE Geral), com indicadores visuais de tendências e alertas de performance.

---

## 📈 **MÉTRICAS E INDICADORES OEE**

### **OEE (Overall Equipment Effectiveness)**

**Conceito**: O OEE é a métrica mais importante para avaliação da eficiência operacional, combinando três aspectos críticos da produção em um único indicador que varia de 0% a 100%.

**Componentes do OEE**:
- **Disponibilidade**: Tempo de produção efetiva vs. tempo total disponível, considerando paradas por anomalias, manutenção e setup
- **Performance**: Velocidade real de produção vs. velocidade teórica máxima, considerando micro-paradas e variações de ciclo
- **Qualidade**: Peças boas produzidas vs. total produzido, excluindo peças com defeito e retrabalhos
- **OEE Geral**: Produto dos três indicadores (Disponibilidade × Performance × Qualidade), representando a eficiência real da máquina

**Interpretação**: OEE acima de 85% é considerado excelente, entre 70-85% é bom, entre 50-70% é aceitável, e abaixo de 50% indica necessidade de melhorias significativas.

### **Dados de Produção**

**Contexto**: Os dados de produção são fundamentais para controle de qualidade, cumprimento de prazos e análise de eficiência operacional.

**Métricas Principais**:
- **Quantidade Planejada**: Meta estabelecida pela OP baseada em demandas do cliente e capacidade da máquina
- **Quantidade Produzida**: Peças efetivamente fabricadas e aprovadas pelo controle de qualidade
- **Quantidade Restante**: Diferença entre planejado e produzido, indicando progresso da OP
- **Peças com Defeito**: Contabilizadas separadamente para cálculo de qualidade e análise de causas

**Importância**: Estes dados permitem controle preciso do progresso, identificação de desvios e tomada de ações corretivas em tempo real.

### **Tempos Operacionais**

**Conceito**: O controle preciso dos tempos operacionais é essencial para cálculo correto do OEE e identificação de oportunidades de melhoria.

**Categorias de Tempo**:
- **Tempo de Produção**: Período ativo produzindo peças com qualidade aceitável, considerado tempo "valor agregado"
- **Tempo de Parada**: Período parado por anomalias, manutenção ou problemas operacionais, considerado tempo "perdido"
- **Tempo de Setup**: Tempo de preparação entre OPs, incluindo troca de ferramentas e configurações, considerado tempo "necessário"
- **Ciclo Real**: Tempo médio por peça produzida, incluindo variações naturais do processo
- **Tempo Total**: Soma de todos os tempos operacionais, base para cálculo de disponibilidade

**Análise**: A análise detalhada destes tempos permite identificação de gargalos, otimização de processos e melhoria contínua da eficiência operacional.

---

## ⚠️ **REGRAS OPERACIONAIS IMPORTANTES**

### **1. Gestão de Operadores**

**Conceito**: O sistema TeepOEE implementa um modelo de responsabilidade única por máquina, garantindo accountability e controle de qualidade.

**Regras Fundamentais**:
- **Um operador por máquina** (não por palete) para evitar conflitos de responsabilidade
- Operador é **global** para toda a máquina e turno, sendo responsável por todas as operações
- **Login obrigatório no início do turno** para ativação do sistema de monitoramento
- **Pode ser alterado durante o turno com autorização** do supervisor para situações excepcionais

**Benefícios**: Este modelo garante responsabilidade clara, facilita análise de performance individual e mantém consistência operacional.

### **2. Estados dos Paletes**

**Conceito**: O sistema de duplo palete opera com regras específicas de coordenação para garantir segurança e eficiência.

**Regras de Coordenação**:
- **Apenas um palete** pode estar ativo por vez para garantir segurança operacional
- **Palete ativo** = em produção ou setup, com todos os sistemas de monitoramento ativos
- **Palete inativo** = aguardando ou sem OP, preparado para próxima operação
- **Troca automática** gerenciada pelo sistema com validações de segurança

**Importância**: Estas regras garantem que não haja conflitos operacionais e que a eficiência seja maximizada através da coordenação inteligente.

### **3. OPs e Paletes**

**Conceito**: A associação entre OPs e paletes segue regras específicas para garantir rastreabilidade e controle operacional.

**Regras de Associação**:
- **OP sempre associada a um palete específico** para manter rastreabilidade completa
- **Palete pode ter OP sem estar na máquina** para preparação antecipada
- **Produção só inicia** quando palete entra na máquina, garantindo controle de qualidade
- **OP fecha automaticamente** ao atingir quantidade planejada, evitando superprodução

**Benefícios**: Estas regras garantem controle preciso de produção, rastreabilidade completa e prevenção de erros operacionais.

### **4. Registro de Paradas**

**Conceito**: O registro de paradas é crítico para análise de eficiência e implementação de melhorias.

**Procedimentos Obrigatórios**:
- **Timer de segurança** de 10 segundos antes do registro para evitar registros acidentais
- **Operador identificado automaticamente** para accountability e análise de performance
- **Máquina permanece parada** mesmo com troca de paletes para manter consistência do OEE
- **Tempo de parada acumula** no cálculo do OEE do turno para análise precisa de eficiência

**Impacto**: O registro correto de paradas é fundamental para identificação de gargalos, análise de causas raiz e desenvolvimento de ações preventivas.

---

## 🔄 **CENÁRIOS DE VALIDAÇÃO RECOMENDADOS**

### **Validação 1: Operação Básica**

**Objetivo**: Validar o funcionamento básico do sistema TeepOEE e familiarizar operadores com a interface.

**Procedimento**:
1. **Login do operador no sistema** com credenciais válidas
2. **Abertura de OP no P1** selecionando ordem do planejamento
3. **Início de produção** após confirmação de setup
4. **Monitoramento de algumas peças** para verificar contadores automáticos
5. **Verificação das métricas OEE** em tempo real

**Critérios de Sucesso**: Sistema operacional, contadores funcionando, métricas OEE calculando corretamente.

### **Validação 2: Troca Automática de Paletes**

**Objetivo**: Validar a funcionalidade principal do sistema de duplo palete e sua eficiência operacional.

**Procedimento**:
1. **OP-001 em produção no P1** com sistema funcionando normalmente
2. **Abertura de OP-002 no P2** (aguarda) enquanto P1 produz
3. **Troca automática de paletes** executada pelo sistema
4. **Verificação de entrada do P2 em setup** com todas as configurações
5. **Início de produção no P2** após confirmação de setup

**Critérios de Sucesso**: Troca automática executada sem erros, continuidade do OEE, tempos de transição otimizados.

### **Validação 3: Registro de Paradas**

**Objetivo**: Validar o sistema de registro de anomalias e seu impacto no cálculo do OEE.

**Procedimento**:
1. **Produção ativa** com sistema funcionando normalmente
2. **Identificação de anomalia** simulada ou real
3. **Registro de parada com classificação** completa (motivo, severidade, descrição)
4. **Correção da anomalia** conforme procedimentos
5. **Retomada de produção** com confirmação no sistema
6. **Verificação do impacto no OEE** e análise de dados

**Critérios de Sucesso**: Registro correto da parada, impacto preciso no OEE, continuidade operacional após retomada.

### **Validação 4: Múltiplas OPs Consecutivas**

**Objetivo**: Validar a eficiência operacional em cenário real de produção com múltiplas ordens.

**Procedimento**:
1. **Abertura de OP-001 no P1** com início de produção
2. **Produção até completar quantidade** planejada
3. **Abertura de OP-002 no P2** durante produção da OP-001
4. **Troca automática de paletes** após conclusão da OP-001
5. **Produção da OP-002** com continuidade do monitoramento
6. **Análise do OEE consolidado** considerando ambas as OPs

**Critérios de Sucesso**: Eficiência operacional otimizada, OEE consolidado preciso, minimização de tempos mortos.

---

## 📋 **CHECKLIST OPERACIONAL**

### **Início do Turno**

**Objetivo**: Estabelecer condições operacionais ideais para início eficiente do turno de trabalho.

**Verificações Obrigatórias**:
- [ ] **Login do operador no sistema TeepOEE** com credenciais válidas e atualizadas
- [ ] **Verificação de OPs disponíveis no planejamento** para sequenciamento otimizado
- [ ] **Validação dos sensores de paletes** para garantir funcionamento correto do sistema
- [ ] **Confirmação do estado inicial da máquina** (limpa, calibrada, operacional)
- [ ] **Definição dos objetivos do turno** baseados em metas de produção e qualidade

**Importância**: Este checklist garante que todas as condições estejam adequadas para operação eficiente e segura.

### **Durante a Operação**

**Objetivo**: Manter controle operacional contínuo e identificar rapidamente qualquer desvio ou oportunidade de melhoria.

**Monitoramento Contínuo**:
- [ ] **Monitoramento contínuo do status da máquina** para identificação imediata de problemas
- [ ] **Verificação dos indicadores de paletes** para controle de posicionamento e estados
- [ ] **Acompanhamento das métricas OEE em tempo real** para análise de performance
- [ ] **Registro adequado de paradas e anomalias** com classificação completa e precisa
- [ ] **Validação das trocas automáticas de paletes** para garantir eficiência operacional

**Benefícios**: Este monitoramento contínuo permite tomada de decisões rápidas e manutenção da eficiência operacional.

### **Fim do Turno**

**Objetivo**: Consolidar dados do turno, analisar performance e preparar condições para o próximo turno.

**Atividades de Encerramento**:
- [ ] **Análise das métricas finais do OEE** para avaliação de performance do turno
- [ ] **Verificação dos logs de eventos do turno** para identificação de padrões e tendências
- [ ] **Documentação de ocorrências e aprendizados** para melhoria contínua
- [ ] **Preparação para o próximo turno** incluindo limpeza e organização do ambiente
- [ ] **Relatório de eficiência operacional** com dados consolidados e recomendações

**Impacto**: Este processo de encerramento garante continuidade operacional e melhoria contínua baseada em dados reais.

---

## 🎓 **OBJETIVOS DE APRENDIZADO**

### **Para Operadores**

**Objetivo Principal**: Dominar a operação eficiente do sistema TeepOEE e contribuir para máxima eficiência operacional.

**Competências Desenvolvidas**:
- **Compreender fluxo de produção com duplo palete** para otimização de sequências e tempos
- **Identificar estados operacionais da máquina** para resposta rápida a situações anômalas
- **Praticar procedimentos de registro de paradas** para contribuir com análise de causas raiz
- **Entender sistema de troca automática de paletes** para aproveitamento máximo da eficiência
- **Dominar interface do TeepOEE** para operação fluida e sem erros

**Impacto**: Operadores competentes contribuem diretamente para aumento do OEE e redução de custos operacionais.

### **Para Supervisores**

**Objetivo Principal**: Utilizar dados do TeepOEE para gestão eficiente de equipes e otimização de processos.

**Competências Desenvolvidas**:
- **Analisar eficiência operacional através do OEE** para tomada de decisões baseada em dados
- **Identificar gargalos e oportunidades de melhoria** através de análise de métricas e tendências
- **Otimizar trocas de paletes e setup** para maximização da eficiência operacional
- **Monitorar indicadores de performance em tempo real** para intervenção proativa
- **Gerenciar equipes baseado em dados** para desenvolvimento de pessoas e processos

**Impacto**: Supervisores eficazes conseguem aumentar significativamente a produtividade e qualidade através de gestão baseada em dados.

### **Para Engenheiros de Processo**

**Objetivo Principal**: Utilizar dados do TeepOEE para otimização contínua de processos e implementação de melhorias.

**Competências Desenvolvidas**:
- **Validar lógica de processo com dados reais** para confirmação de eficiência teórica
- **Testar cenários complexos de produção** para identificação de oportunidades de otimização
- **Analisar dados de produção para otimização** através de análise estatística e tendências
- **Refinar procedimentos baseado em métricas** para melhoria contínua de processos
- **Implementar melhorias contínuas** baseadas em evidências e dados quantitativos

**Impacto**: Engenheiros competentes conseguem implementar melhorias que resultam em ganhos significativos de eficiência e redução de custos.

---

## 📞 **SUPORTE E ESCLARECIMENTOS**

### **Sobre o TeepOEE - Duplo Palete**

O **TeepOEE - Duplo Palete** foi desenvolvido especificamente para **monitoramento real de máquinas industriais** com sistema de duplo palete. Este sistema representa uma solução completa para controle de eficiência operacional em ambientes de produção de alta complexidade.

### **Recursos de Suporte**

**Para Dúvidas Operacionais**:
- **Funcionamento**: Consulte este guia operacional completo
- **Procedimentos**: Siga os cenários de validação detalhados
- **Métricas OEE**: Analise os indicadores em tempo real através da interface
- **Problemas técnicos**: Verifique logs de eventos do sistema para diagnóstico
- **Integração**: Consulte documentação técnica específica para implementação

### **Importância do Sistema**

**Contexto Industrial**: Este é um **sistema de produção real** desenvolvido para monitoramento e controle de eficiência operacional em ambientes industriais críticos. Todas as métricas e dados coletados são utilizados para:

- **Análise de performance** em tempo real e histórica
- **Tomada de decisões operacionais** baseadas em dados precisos
- **Identificação de oportunidades de melhoria** através de análise de tendências
- **Otimização contínua de processos** para maximização da eficiência
- **Gestão de equipes** baseada em indicadores objetivos de performance

### **Compromisso com a Qualidade**

O TeepOEE foi desenvolvido com foco na **confiabilidade**, **precisão** e **usabilidade**, garantindo que operadores, supervisores e engenheiros tenham acesso a informações precisas e acionáveis para otimização contínua da eficiência operacional.

---

*Documento criado para orientação operacional do TeepOEE - Sistema de Duplo Palete*  
*Versão: 1.0 | Data: 2024 | Foco: Operação Industrial*
