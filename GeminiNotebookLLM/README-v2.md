# 🚀 Repositório "Nota 10" — Jornada CCNA 200-301 & Caderno Temático

Repositório estruturado para documentação de estudos, engenharia de prompts, curadoria de fontes e preparação prática para a certificação **Cisco CCNA 200-301** (meta de realização: **Janeiro de 2026**).

---

## 🎯 1. Contexto e Objetivos

### Contexto do Projeto
Este projeto foi desenvolvido como um **caderno temático de engenharia de redes e certificação**, focado no exame **Cisco CCNA 200-301 (v1.1)** [3]. A estratégia combina estudo acadêmico, laboratórios práticos e otimização financeira através da conquista do **voucher de desconto NetAcad (até 58% OFF)** [13].

### Objetivos de Estudo
1. **Domínio Técnico:** Absorver os 6 domínios oficiais da Cisco (Fundamentos de Rede, Acesso à Rede, Conectividade IP, Serviços IP, Fundamentos de Segurança e Automação/Programabilidade) [3].
2. **Conquista do Desconto Oficial:** Alcançar nota igual ou superior a 70% na primeira tentativa do exame final do curso **CCNA 3 (ENSA)** na Cisco Networking Academy [13].
3. **Prática Intensiva:** Executar e documentar cenários de laboratório usando o simulador **Cisco Packet Tracer** (com base em pacotes de 357 laboratórios práticos) [4].
4. **Gestão de Tempo:** Cumprir um plano de 16 semanas adaptado à rotina de 1-2h/dia em dias úteis e 4-5h/dia aos fins de semana.

---

## 📚 2. Curadoria de Fontes (Fontes Abertas Selecionadas)

As seguintes fontes foram selecionadas e integradas ao projeto para fundamentação teórica e prática:

1. 📄 **[PDF] Guia de Estudo CCNA 200-301 (elhacker.INFO / Cisco Press)**
   * *Descrição:* Material de referência teórica abrangendo conceitos de switching, roteamento, IPv4/IPv6 e segurança [22].
2. 🔗 **[URL] 200-301 CCNA Exam Topics and Study Guide (Cisco Learning Network)**
   * *Descrição:* Documento oficial com o blueprint da prova e os pesos percentuais de cada tópico do exame [3].
3. 🔗 **[URL] 357 Laboratórios no Packet Tracer (Café com Redes)**
   * *Descrição:* Repositório prático de arquivos `.pkt` cobrindo desde configurações básicas de CLI até topologias OSPF e EtherChannel [4].
4. 📄 **[PDF] CCNAv7 SRWE — Escopo e Sequência (Cisco Networking Academy)**
   * *Descrição:* Ementa oficial do módulo 2 do NetAcad detalhando VLANs, Spanning Tree, RSTP, WLC e DHCP [8].
5. 🔗 **[URL] Cursos Gratuitos DLTec do Brasil com Certificado**
   * *Descrição:* Cursos de nivelamento em Modelo OSI, Linux, Cloud e Fundamentos de Cisco IOS [16].

---

## 🛠️ 3. Engenharia de Prompts e "Cicatrizes" (Lessons Learned & Troubleshooting)

Para extrair o máximo de precisão da Inteligência Artificial durante a elaboração deste plano e dos materiais de revisão, foram testadas diferentes abordagens de prompts.

### Prompts Testados & Evolução

| Fase | Prompt Inicial (Genérico) | Prompt Otimizado (Engenharia) | Resultado Obtido / Melhoria |
| :--- | :--- | :--- | :--- |
| **Cronograma** | *"Monte um plano de estudo para o CCNA."* | *"Crie um cronograma de 16 semanas para a prova CCNA 200-301 em janeiro, considerando 1-2h em dias úteis e 4-5h nos fins de semana, incluindo o curso NetAcad para o voucher de 58%."* | Mudou de uma lista vaga de tópicos para uma matriz diária e semanal viável com metas específicas por módulo. |
| **Comandos IOS** | *"Quais os comandos de switch no CCNA?"* | *"Liste os comandos IOS essenciais de verificação (`show`) e configuração para VLANs, Trunking, OSPF e Port Security no Packet Tracer, organizados por protocolo."* | Gerou um guia rápido direto para prática em CLI sem enrolação teórica. |
| **Subnetting** | *"Me explique cálculo de sub-rede."* | *"Crie um passo a passo para cálculo mental de sub-redes IPv4 VLSM com blocos /24 a /30, focado em resolver questões do CCNA em menos de 1 minuto."* | Forneceu métodos práticos de tabela de potências de 2 aplicáveis ao exame oficial. |

### 🩹 "Cicatrizes" & Troubleshooting (Desafios Encontrados)
* **Desafio 1: Respostas Genéricas em Carga Horária.** 
  * *Problema:* A IA inicialmente sugeria jornadas de 4 horas diárias, incompatíveis com a rotina de trabalho.
  * *Solução:* Especificação estrita de restrições de tempo no prompt (diferenciando dias úteis de finais de semana).
* **Desafio 2: Mistura de Escopos de Provas Antigas (Ex: CCNA 640-801 vs 200-301).**
  * *Problema:* Algumas fontes traziam nomenclaturas antigas de exames Cisco.
  * *Solução:* Forçar a IA a validar os tópicos contra o blueprint oficial v1.1 do exame 200-301 [3].
* **Desafio 3: Foco Excessivo em Teoria sem Prática.**
  * *Problema:* O plano inicial gerado não pontuava quando abrir o Packet Tracer.
  * *Solução:* Incluir a regra de "Teoria durante a semana, Hands-on / Labs no sábado e Simulados no domingo".

---

## 📖 4. Miniguia de Estudo (Entrega Final)

### A. Resumos Estruturados por Domínio

#### 1. Network Fundamentals (20%) [3]
* **Modelo OSI vs TCP/IP:** Camadas 1 a 7 vs Aplicação, Transporte, Internet e Acesso à Rede.
* **IPv4 & Subnetting:** Classes A, B, C; CIDR; Máscaras de tamanho variável (VLSM); Broadcast, Network e Host IDs.
* **IPv6:** Unicast (Global, Link-Local, Unique Local), Multicast, Anycast; Autoconfiguração SLAAC e DHCPv6.

#### 2. Network Access (20%) [3]
* **VLANs & Trunking:** 802.1Q tagging, Native VLAN, VTP (Modos Server/Client/Transparent).
* **Spanning Tree Protocol (STP):** 802.1D (STP), 802.1w (RSTP). Estados de porta: Blocking, Listening, Learning, Forwarding.
* **EtherChannel:** Agregação de links via LACP (802.3ad) ou PAgP (Proprietário Cisco).
* **WLAN & WLC:** Arquitetura CAPWAP, SSIDs, WPA2/WPA3 Enterprise (802.1X/RADIUS), gerenciamento via Wireless LAN Controller.

#### 3. IP Connectivity (25%) [3]
* **Tabela de Roteamento:** Longest Prefix Match (Regra do prefixo mais específico), Distância Administrativa (AD): Conectada (0), Estática (1), eBGP (20), OSPF (110), RIP (120).
* **OSPFv2 (Single-Area):** Router ID, Hellos, LSA Type 1 e 2, Formação de Adjacência (Init, 2-Way, ExStart, Exchange, Loading, Full), Eleição de DR/BDR em redes Broadcast.

#### 4. IP Services (10%) [3]
* **NAT/PAT:** Static NAT, Dynamic NAT, PAT (Overload).
* **DHCP & First Hop Redundancy:** DHCP Server/Relay Agent, conceitos de FHRP (HSRP/VRRP).
* **NTP & SNMP:** Sincronização de relógio (Stratum), monitoramento via SNMPv2c/v3.

#### 5. Security Fundamentals (15%) [3]
* **Listas de Controle de Acesso (ACLs):** Standard (1-99 / 1300-1399 — filtra por IP de origem perto do destino) vs Extended (100-199 / 2000-2699 — filtra por protocolo/porta perto da origem).
* **L2 Security:** Port Security (Sticky MAC), DHCP Snooping, Dynamic ARP Inspection (DAI).
* **AAA & VPNs:** Authentication, Authorization, Accounting; IPSec site-to-site e remote access.

#### 6. Automation and Programmability (10%) [3]
* **Arquitera SDN:** Plano de Controle (Control Plane) vs Plano de Dados (Data Plane); Overlay vs Underlay; Cisco DNA Center.
* **APIs REST:** Métodos HTTP (GET, POST, PUT, DELETE), Códigos de Status (200 OK, 201 Created, 400 Bad Request, 404 Not Found).
* **Formatos de Dados:** JSON (chave:valor), XML, YAML.

---

### B. Glossário de Conceitos Chave

* **ACL (Access Control List):** Conjunto de regras aplicadas a interfaces de roteadores/switches para permitir ou negar tráfego com base em critérios de rede.
* **AD (Administrative Distance):** Valor de confiabilidade atribuído a uma fonte de roteamento (quanto menor o valor, mais preferida é a rota).
* **CAPWAP:** Protocolo de túnel que permite a um WLC gerenciar Access Points leves (Lightweight APs).
* **DAI (Dynamic ARP Inspection):** Recurso de segurança L2 que valida pacotes ARP na rede para prevenir ataques de ARP Spoofing/Poisoning.
* **DHCP Snooping:** Recurso que atua como firewall de camada 2, filtrando mensagens DHCP não autorizadas (Rogue DHCP).
* **LACP (Link Aggregation Control Protocol):** Protocolo padrão IEEE (802.3ad) usado para negociar o agrupamento de links físicos em um EtherChannel.
* **OSPF (Open Shortest Path First):** Protocolo de roteamento Link-State dinâmico que utiliza o algoritmo de Dijkstra para calcular a menor rota baseada em custo (banda).
* **Port Security:** Recurso de switch que limita o número de endereços MAC permitidos em uma porta para impedir acessos não autorizados.
* **RSTP (Rapid Spanning Tree Protocol - 802.1w):** Evolução do STP tradicional que reduz o tempo de convergência da rede de 30-50s para poucos segundos.
* **VLSM (Variable Length Subnet Mask):** Técnica que permite dividir um espaço de endereçamento IP em sub-redes de tamanhos diferentes, otimizando o uso de IPs.

---

### C. Prompts Reutilizáveis para Estudos Futuros

Você pode copiar e colar os prompts abaixo no seu assistente de IA para revisar e praticar ao longo das 16 semanas:

#### 🧪 Prompt 1: Gerador de Laboratório Prático (Packet Tracer)
> *"Atue como um instrutor Cisco CCNA. Crie um cenário de laboratório para o Packet Tracer focado em [TÓPICO, ex: Inter-VLAN Routing com Router-on-a-Stick]. Forneça: 1) A topologia e dispositivos necessários; 2) O objetivo de negócio; 3) A tabela de desempenhos/IPs; 4) O passo a passo de comandos IOS para configuração; 5) Os comandos `show` para validação do laboratório."*

#### 📝 Prompt 2: Simulado Estilo Exame Oficial
> *"Elabore 3 questões no formato exato da prova Cisco CCNA 200-301 sobre [TÓPICO, ex: OSPFv2 e DR/BDR]. Cada questão deve ter 4 alternativas (A, B, C, D) com apenas 1 correta. Ao final, apresente o gabarito comentado detalhando o porquê da alternativa correta e o erro de cada uma das alternativas incorretas."*

#### 🔍 Prompt 3: Troubleshooting de Comando IOS
> *"Dado a seguinte saída de comando IOS no switch/roteador Cisco: [COLE A SAÍDA DO COMANDO `SHOW` AQUI], identifique qual é a falha de configuração de rede existente, explique a causa raiz do problema e forneça os comandos exatos de CLI para corrigir."*

#### 📐 Prompt 4: Treino Rápido de Subnetting
> *"Gere 5 exercícios de cálculo de sub-rede IPv4 VLSM com nível de dificuldade progressivo. Ao final, exiba a resposta formatada em uma tabela contendo: Endereço de Rede, Primeiro IP Válido, Último IP Válido, Endereço de Broadcast e Máscara Decimal."*

---

## 📅 5. Estrutura do Repositório no GitHub

```text
├── 📂 01-contexto-e-fontes/      # Links das fontes abertas, PDFs e blueprint oficial
├── 📂 02-engenharia-prompts/     # Histórico de testes de prompts e cicatrizes
├── 📂 03-miniguia-estudo/        # Resumos por domínio e glossário técnico
├── 📂 04-laboratorios-pkt/       # Arquivos .pkt e scripts de configuração IOS
├── 📂 05-simulados-e-prompts/    # Prompts reutilizáveis e baterias de questões
└── README.md                     # Documentação principal consolidada
```

---

*Projeto construído para a certificação Cisco CCNA 200-301 — Meta: Janeiro/2026 | Desconto NetAcad 58% OFF*
