# Awesome Incident Response [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> Uma lista curada de ferramentas e recursos para resposta a incidentes de segurança, destinada a ajudar analistas de segurança e equipes de [DFIR](http://www.acronymfinder.com/Digital-Forensics%2c-Incident-Response-%28DFIR%29.html).

Equipes de Forense Digital e Resposta a Incidentes são grupos de pessoas em uma organização responsáveis por gerenciar a resposta a um incidente de segurança, incluindo a coleta de evidências do incidente, a remediação de seus efeitos e a implementação de controles para evitar que o incidente se repita no futuro. Essa lista é baseada no fork citado acima, porém atualizei com algumas ferramentas que utilizo no dia a dia e traduzi para a comunidade brasileira.

## Conteúdo

- [Emulação de Adversário](#emulação-de-adversário)
- [Ferramentas Tudo-em-Um](#ferramentas-tudo-em-um)
- [Livros](#livros)
- [Ferramentas de Criação de Imagem de Disco](#ferramentas-de-criação-de-imagem-de-disco)
- [Coleta de Evidências](#coleta-de-evidências)
- [Gerenciamento de Incidentes](#gerenciamento-de-incidentes)
- [Bases de Conhecimento](#bases-de-conhecimento)
- [Distribuições Linux](#distribuições-linux)
- [Coleta de Evidências em Linux](#coleta-de-evidências-em-linux)
- [Ferramentas de Análise de Logs](#ferramentas-de-análise-de-logs)
- [Ferramentas de Análise de Memória](#ferramentas-de-análise-de-memória)
- [Ferramentas de Imagem de Memória](#ferramentas-de-imagem-de-memória)
- [Coleta de Evidências em OSX](#coleta-de-evidências-em-osx)
- [Outras Listas](#outras-listas)
- [Outras Ferramentas](#outras-ferramentas)
- [Playbooks](#playbooks)
- [Ferramentas de Dump de Processos](#ferramentas-de-dump-de-processos)
- [Ferramentas de Sandbox/Engenharia Reversa](#ferramentas-de-sandboxengenharia-reversa)
- [Ferramentas de Scanner](#ferramentas-de-scanner)
- [Ferramentas de Linha do Tempo](#ferramentas-de-linha-do-tempo)
- [Vídeos](#vídeos)
- [Coleta de Evidências em Windows](#coleta-de-evidências-em-windows)
- [🤖 IA & LLM para IR](#-ia--llm-para-ir)

## Coleção de Ferramentas de IR

### Emulação de Adversário

* [APTSimulator](https://github.com/NextronSystems/APTSimulator) - Script em lote do Windows que usa um conjunto de ferramentas e arquivos de saída para fazer um sistema parecer comprometido.
* [Atomic Red Team (ART)](https://github.com/redcanaryco/atomic-red-team) - Testes de detecção pequenos e altamente portáveis mapeados para o framework MITRE ATT&CK.
* [AutoTTP](https://github.com/jymcheong/AutoTTP) - Táticas, Técnicas e Procedimentos Automatizados. Reexecuta sequências complexas manualmente para testes de regressão, avaliações de produtos e geração de dados para pesquisadores.
* [Caldera](https://github.com/mitre/caldera) - Sistema automatizado de emulação de adversário que executa comportamento adversarial pós-comprometimento em redes Windows Enterprise.
* [DumpsterFire](https://github.com/TryCatchHCF/DumpsterFire) - Ferramenta modular, orientada por menu e multiplataforma para construir eventos de segurança repetíveis, com atraso de tempo e distribuídos.
* [Metta](https://github.com/uber-common/metta) - Ferramenta de preparação de segurança da informação para simulação adversarial.
* [Network Flight Simulator](https://github.com/alphasoc/flightsim) - Utilitário leve usado para gerar tráfego de rede malicioso.
* [Red Team Automation (RTA)](https://github.com/endgameinc/RTA) - Framework de scripts projetado para permitir que equipes azuis testem suas capacidades de detecção contra tradecraft malicioso.
* [RedHunt-OS](https://github.com/redhuntlabs/RedHunt-OS) - Máquina virtual para emulação de adversário e caça a ameaças.

### Ferramentas Tudo-em-Um

* [Belkasoft Evidence Center](https://belkasoft.com/ec) - O kit de ferramentas extrai rapidamente evidências digitais de múltiplas fontes.
* [CimSweep](https://github.com/PowerShellMafia/CimSweep) - Conjunto de ferramentas baseadas em CIM/WMI para resposta a incidentes e operações de caça remotamente em Windows.
* [Cyber Triage](http://www.cybertriage.com) - Coleta e analisa dados do host para determinar se está comprometido. O sistema de pontuação e o motor de recomendação permitem focar rapidamente em artefatos importantes.
* [Dissect](https://github.com/fox-it/dissect) - Framework e conjunto de ferramentas de forense digital e resposta a incidentes da Fox-IT (NCC Group).
* [Doorman](https://github.com/mwielgoszewski/doorman) - Gerenciador de frota osquery que permite gerenciamento remoto de configurações do osquery.
* [Falcon Orchestrator](https://github.com/CrowdStrike/falcon-orchestrator) - Aplicação extensível baseada em Windows que fornece automação de fluxo de trabalho, gerenciamento de casos e funcionalidade de resposta de segurança.
* [Flare](https://github.com/fireeye/flare-vm) - Distribuição de segurança baseada em Windows totalmente personalizável para análise de malware, resposta a incidentes e testes de penetração.
* [Fleetdm](https://github.com/fleetdm/fleet) - Plataforma de monitoramento de hosts de última geração voltada para especialistas em segurança.
* [GRR Rapid Response](https://github.com/google/grr) - Framework de resposta a incidentes focado em forense remota ao vivo.
* [IRIS](https://github.com/dfir-iris/iris-web) - Plataforma colaborativa web para analistas de resposta a incidentes.
* [Kuiper](https://github.com/DFIRKuiper/Kuiper) - Plataforma de Investigação Forense Digital
* [Limacharlie](https://www.limacharlie.io/) - Plataforma de segurança de endpoint com ambiente de baixo nível multiplataforma para gerenciar módulos em memória.
* [Matano](https://github.com/matanolabs/matano) - Plataforma open source de lago de segurança serverless na AWS com Apache Iceberg e detecções Python em tempo real.
* [MozDef](https://github.com/mozilla/MozDef) - Automatiza o processo de tratamento de incidentes de segurança.
* [MutableSecurity](https://github.com/MutableSecurity/mutablesecurity) - Programa CLI para automatizar a configuração, setup e uso de soluções de cibersegurança.
* [nightHawk](https://github.com/biggiesmallsAG/nightHawkResponse) - Aplicação para apresentação assíncrona de dados forenses usando ElasticSearch.
* [osquery](https://osquery.io/) - Faça perguntas sobre sua infraestrutura Linux e macOS usando uma linguagem de consulta similar a SQL.
* [Redline](https://www.fireeye.com/services/freeware/redline.html) - Fornece capacidades investigativas de host através de análise de memória e arquivos.
* [SOC Multi-tool](https://github.com/zdhenard42/SOC-Multitool) - Extensão de navegador que agiliza investigações para profissionais de segurança.
* [The Sleuth Kit & Autopsy](http://www.sleuthkit.org) - Ferramenta baseada em Unix e Windows para análise forense de computadores.
* [TheHive](https://thehive-project.org/) - Solução open source 3-em-1 escalável para SOCs, CSIRTs, CERTs.
* [Velociraptor](https://github.com/Velocidex/velociraptor) - Ferramenta de visibilidade e coleta de endpoint.
* [X-Ways Forensics](http://www.x-ways.net/forensics/) - Ferramenta forense para clonagem e imagem de disco.
* [Zentral](https://github.com/zentralopensource/zentral) - Combina os recursos de inventário de endpoint do osquery com um framework flexível de notificação e ação.

### Livros

* [Applied Incident Response](https://www.amazon.com/Applied-Incident-Response-Steve-Anson/dp/1119560268/) - Livro de Steve Anson sobre Resposta a Incidentes.
* [Art of Memory Forensics](https://www.amazon.com/Art-Memory-Forensics-Detecting-Malware/dp/1118825098/) - Detecção de Malware e Ameaças em Memória Windows, Linux e Mac.
* [Crafting the InfoSec Playbook](https://www.amazon.com/Crafting-InfoSec-Playbook-Security-Monitoring/dp/1491949406) - Plano Mestre de Monitoramento de Segurança e Resposta a Incidentes.
* [Digital Forensics and Incident Response](https://www.amazon.com/Digital-Forensics-Incident-Response-techniques/dp/183864900X) - Técnicas e procedimentos de resposta a incidentes para ameaças cibernéticas modernas.
* [Practical Memory Forensics](https://www.amazon.com/Practical-Memory-Forensics-Jumpstart-effective/dp/1801070334) - O guia definitivo para praticar forense de memória.
* [The Practice of Network Security Monitoring](http://www.amazon.com/gp/product/1593275099) - Livro de Richard Bejtlich sobre IR.

### Ferramentas de Criação de Imagem de Disco

* [AccessData FTK Imager](http://accessdata.com/product-download/?/support/adownloads#FTKImager) - Ferramenta forense para visualizar dados recuperáveis de um disco.
* [Bitscout](https://github.com/vitaly-kamluk/bitscout) - Construa uma imagem LiveCD/LiveUSB personalizável e totalmente confiável para forense digital remota.
* [GetData Forensic Imager](http://www.forensicimager.com/) - Programa baseado em Windows que adquire, converte ou verifica uma imagem forense.
* [Guymager](http://guymager.sourceforge.net) - Imageador forense gratuito para aquisição de mídia no Linux.
* [Magnet ACQUIRE](https://www.magnetforensics.com/magnet-acquire/) - Permite vários tipos de aquisições de disco em Windows, Linux, OS X e sistemas operacionais móveis.

### Coleta de Evidências

* [Acquire](https://github.com/fox-it/acquire) - Colete rapidamente artefatos forenses de imagens de disco ou de um sistema ao vivo.
* [artifactcollector](https://github.com/forensicanalysis/artifactcollector) - Fornece software que coleta artefatos forenses em sistemas.
* [bulk_extractor](https://github.com/simsong/bulk_extractor) - Examina uma imagem de disco, arquivo ou diretório e extrai informações úteis sem analisar o sistema de arquivos.
* [Cold Disk Quick Response](https://github.com/rough007/CDQR) - Lista simplificada de analisadores para analisar rapidamente um arquivo de imagem forense.
* [CyLR](https://github.com/orlikoski/CyLR) - Coleta artefatos forenses de hosts com sistemas de arquivos NTFS de forma rápida e segura.
* [Forensic Artifacts](https://github.com/ForensicArtifacts/artifacts) - Repositório de Artefatos de Forense Digital.
* [ir-rescue](https://github.com/diogo-fernan/ir-rescue) - Script em lote do Windows e script Bash do Unix para coletar abrangentemente dados forenses do host.
* [Live Response Collection](https://www.brimorlabs.com/tools/) - Ferramenta automatizada que coleta dados voláteis de sistemas operacionais Windows, OSX e *nix.
* [Margarita Shotgun](https://github.com/ThreatResponse/margaritashotgun) - Utilitário de linha de comando para paralelizar aquisição remota de memória.
* [SPECTR3](https://github.com/alpine-sec/SPECTR3) - Adquire, faz triagem e investiga evidências remotas via acesso iSCSI portátil somente leitura.
* [UAC](https://github.com/tclahr/uac) - Coletor de Artefatos Unix-like para Resposta a Incidentes.

### Gerenciamento de Incidentes

* [Catalyst](https://github.com/SecurityBrewery/catalyst) - Sistema SOAR gratuito que ajuda a automatizar o tratamento de alertas e processos de resposta a incidentes.
* [CyberCPR](https://www.cybercpr.com) - Ferramenta de gerenciamento de incidentes comunitária e comercial com Need-to-Know embutido.
* [CORTEX XSOAR](https://www.paloaltonetworks.com/cortex/xsoar) - Plataforma de orquestração, automação e resposta de segurança da Paloalto com gerenciamento completo do ciclo de vida de incidentes.
* [DFTimewolf](https://github.com/log2timeline/dftimewolf) - Framework para orquestrar coleta forense, processamento e exportação de dados.
* [DFIRTrack](https://github.com/dfirtrack/dfirtrack) - Aplicação de rastreamento de Resposta a Incidentes lidando com casos e tarefas com sistemas afetados.
* [Fast Incident Response (FIR)](https://github.com/certsocietegenerale/FIR/) - Plataforma de gerenciamento de incidentes de cibersegurança projetada com agilidade e velocidade em mente.
* [RTIR](https://www.bestpractical.com/rtir/) - Request Tracker para Resposta a Incidentes, destinado a equipes de segurança de computadores.
* [Sandia Cyber Omni Tracker (SCOT)](https://github.com/sandialabs/scot) - Ferramenta de colaboração e captura de conhecimento para Resposta a Incidentes.
* [Shuffle](https://github.com/frikky/Shuffle) - Plataforma de automação de segurança de uso geral focada em acessibilidade.
* [threat_note](https://github.com/defpoint/threat_note) - Notebook de investigação leve para registrar e recuperar indicadores.
* [Zenduty](https://www.zenduty.com) - Plataforma de gerenciamento de incidentes fornecendo alerta de incidentes de ponta a ponta, gerenciamento de plantão e orquestração de resposta.

### Bases de Conhecimento

* [Digital Forensics Artifact Knowledge Base](https://github.com/ForensicArtifacts/artifacts-kb) - Base de Conhecimento de Artefatos de Forense Digital.
* [Windows Events Attack Samples](https://github.com/sbousseaden/EVTX-ATTACK-SAMPLES) - Amostras de Ataque em Eventos do Windows.
* [Windows Registry Knowledge Base](https://github.com/libyal/winreg-kb) - Base de Conhecimento do Registro do Windows.

### Distribuições Linux

* [The Appliance for Digital Investigation and Analysis (ADIA)](https://forensics.cert.org/#ADIA) - Appliance baseado em VMware para investigação e aquisição digital.
* [Computer Aided Investigative Environment (CAINE)](http://www.caine-live.net/index.html) - Contém inúmeras ferramentas para investigadores durante a análise.
* [CCF-VM](https://github.com/rough007/CCF-VM) - Máquina Virtual Forense CyLR CDQR: solução tudo-em-um para analisar dados coletados.
* [NST - Network Security Toolkit](https://sourceforge.net/projects/nst/files/latest/download?source=files) - Distribuição Linux com uma vasta coleção de aplicações de segurança de rede open source.
* [PALADIN](https://sumuri.com/software/paladin/) - Distribuição Linux modificada para realizar várias tarefas forenses de maneira forensemente sólida.
* [Security Onion](https://github.com/Security-Onion-Solutions/security-onion) - Distro Linux especial voltada para monitoramento de segurança de rede.
* [SANS Investigative Forensic Toolkit (SIFT) Workstation](http://digital-forensics.sans.org/community/downloads) - Demonstra capacidades avançadas de resposta a incidentes e técnicas forenses digitais.

### Coleta de Evidências em Linux

* [FastIR Collector Linux](https://github.com/SekoiaLab/Fastir_Collector_Linux) - Coleta diferentes artefatos em Linux ao vivo e registra resultados em arquivos CSV.
* [MAGNET DumpIt](https://github.com/MagnetForensics/dumpit-linux) - Ferramenta open source de aquisição de memória rápida para Linux escrita em Rust.

### Ferramentas de Análise de Logs

* [AppCompatProcessor](https://github.com/mbevilacqua/appcompatprocessor) - Extrai valor adicional de dados AppCompat / AmCache em toda a empresa.
* [APT Hunter](https://github.com/ahmedkhlief/APT-Hunter) - Ferramenta de Caça a Ameaças para logs de eventos do Windows.
* [Chainsaw](https://github.com/countercept/chainsaw) - Fornece poderosa capacidade de 'primeira resposta' para identificar rapidamente ameaças em logs de eventos do Windows.
* [Hayabusa](https://github.com/Yamato-Security/hayabusa) - Gerador rápido de linha do tempo forense de logs de eventos do Windows e ferramenta de caça a ameaças.
* [Logdissect](https://github.com/dogoncouch/logdissect) - Utilitário CLI e API Python para analisar arquivos de log e outros dados.
* [LogonTracer](https://github.com/JPCERTCC/LogonTracer) - Ferramenta para investigar logon malicioso do Windows visualizando e analisando logs de eventos do Windows.
* [Sigma](https://github.com/SigmaHQ/sigma) - Formato de assinatura genérico para sistemas SIEM com conjunto extenso de regras.
* [SysmonSearch](https://github.com/JPCERTCC/SysmonSearch) - Torna a análise de logs de eventos do Windows mais eficaz através da agregação de logs de eventos.
* [WELA](https://github.com/Yamato-Security/WELA) - Analisador de Log de Eventos do Windows visa ser o canivete suíço para logs de eventos do Windows.
* [YAMAGoya](https://github.com/JPCERTCC/YAMAGoya) - Ferramenta de monitoramento de cliente em tempo real usando regras Sigma e YARA via ETW.
* [Zircolite](https://github.com/wagga40/Zircolite) - Ferramenta de detecção baseada em SIGMA autônoma e rápida para EVTX ou JSON.

### Ferramentas de Análise de Memória

* [AVML](https://github.com/microsoft/avml) - Ferramenta portátil de aquisição de memória volátil para Linux.
* [Evolve](https://github.com/JamesHabben/evolve) - Interface web para o Framework de Forense de Memória Volatility.
* [inVtero.net](https://github.com/ShaneK2/inVtero.net) - Análise avançada de memória para Windows x64 com suporte a hipervisor aninhado.
* [LiME](https://github.com/504ensicsLabs/LiME) - Módulo de Kernel Carregável para aquisição de memória volátil de Linux e dispositivos baseados em Linux.
* [MalConfScan](https://github.com/JPCERTCC/MalConfScan) - Plugin Volatility que extrai dados de configuração de malware conhecido.
* [Memoryze](https://www.fireeye.com/services/freeware/memoryze.html) - Software forense de memória gratuito que ajuda respondentes de incidentes a encontrar o mal na memória ao vivo.
* [MemProcFS](https://github.com/ufrisk/MemProcFS) - Maneira fácil e conveniente de visualizar memória física como arquivos em um sistema de arquivos virtual.
* [Orochi](https://github.com/LDO-CERT/orochi) - Framework open source para análise colaborativa de dump de memória forense.
* [Volatility 3](https://github.com/volatilityfoundation/volatility3) - O framework de extração de memória volátil (sucessor do Volatility 2).
* [VolatilityBot](https://github.com/mkorman90/VolatilityBot) - Ferramenta de automação para pesquisadores que elimina tarefas manuais da fase de extração binária.
* [VolDiff](https://github.com/aim4r/VolDiff) - Análise de Pegada de Memória de Malware baseada em Volatility.

### Ferramentas de Imagem de Memória

* [Belkasoft Live RAM Capturer](http://belkasoft.com/ram-capturer) - Pequena ferramenta forense gratuita para extrair confiavelmente todo o conteúdo da memória volátil do computador.
* [Linux Memory Grabber](https://github.com/halpomeranz/lmg/) - Script para despejar memória Linux e criar perfis Volatility.
* [MAGNET DumpIt](https://www.magnetforensics.com/resources/magnet-dumpit-for-windows) - Ferramenta rápida de aquisição de memória para Windows (x86, x64, ARM64).
* [Magnet RAM Capture](https://www.magnetforensics.com/free-tool-magnet-ram-capture/) - Ferramenta de imagem gratuita projetada para capturar a memória física do computador de um suspeito.
* [OSForensics](http://www.osforensics.com/) - Ferramenta para adquirir memória ao vivo em sistemas de 32 e 64 bits.

### Coleta de Evidências em OSX

* [Knockknock](https://objective-see.com/products/knockknock.html) - Exibe itens persistentes que estão configurados para executar automaticamente no OSX.
* [macOS Artifact Parsing Tool (mac_apt)](https://github.com/ydkhatri/mac_apt) - Framework forense baseado em plugins para triagem rápida de mac.
* [OSX Auditor](https://github.com/jipegit/OSXAuditor) - Ferramenta forense gratuita para Mac OS X.
* [OSX Collector](https://github.com/yelp/osxcollector) - Derivado do OSX Auditor para resposta ao vivo.
* [The ESF Playground](https://themittenmac.com/the-esf-playground/) - Ferramenta para visualizar eventos no Apple Endpoint Security Framework (ESF) em tempo real.

### Outras Listas

* [Awesome Event IDs](https://github.com/stuhli/awesome-event-ids) - Coleção de recursos de Event ID úteis para Forense Digital e Resposta a Incidentes.
* [Awesome Forensics](https://github.com/cugu/awesome-forensics) - Uma lista curada de ferramentas e recursos de análise forense.
* [Didier Stevens Suite](https://github.com/DidierStevens/DidierStevensSuite) - Coleção de ferramentas.
* [Eric Zimmerman Tools](https://ericzimmerman.github.io/) - Lista atualizada de ferramentas forenses criadas por Eric Zimmerman.
* [List of various Security APIs](https://github.com/deralexxx/security-apis) - Lista coletiva de APIs JSON públicas para uso em segurança.

### Outras Ferramentas

* [Cortex](https://thehive-project.org) - Analise observáveis como endereços IP e e-mail, URLs, nomes de domínio, arquivos ou hashes um por um ou em massa.
* [Crits](https://crits.github.io/) - Ferramenta baseada na web que combina um motor analítico com um banco de dados de ameaças cibernéticas.
* [Diffy](https://github.com/Netflix-Skunkworks/diffy) - Ferramenta DFIR desenvolvida pelo SIRT da Netflix para escopo de comprometimento em instâncias de nuvem.
* [domfind](https://github.com/diogo-fernan/domfind) - Crawler DNS em Python para encontrar nomes de domínio idênticos sob diferentes TLDs.
* [Fileintel](https://github.com/keithjjones/fileintel) - Puxe inteligência por hash de arquivo.
* [HELK](https://github.com/Cyb3rWard0g/HELK) - Plataforma de Caça a Ameaças.
* [Hindsight](https://github.com/obsidianforensics/hindsight) - Forense de histórico de internet para Google Chrome/Chromium.
* [Hostintel](https://github.com/keithjjones/hostintel) - Puxe inteligência por host.
* [imagemounter](https://github.com/ralphje/imagemounter) - Utilitário de linha de comando e pacote Python para facilitar a (des)montagem de imagens de disco forenses.
* [Kansa](https://github.com/davehull/Kansa/) - Framework modular de resposta a incidentes em PowerShell.
* [MFT Browser](https://github.com/kacos2000/MFT_Browser) - Reconstrução da árvore de diretórios MFT e informações de registro.
* [Munin](https://github.com/Neo23x0/munin) - Verificador de hash online para VirusTotal e outros serviços.
* [PowerSponse](https://github.com/swisscom/PowerSponse) - Módulo PowerShell focado em contenção direcionada e remediação durante resposta a incidentes de segurança.
* [PyaraScanner](https://github.com/nogoodconfig/pyarascanner) - Script Python de varredura YARA multi-threaded many-rules to many-files.
* [rastrea2r](https://github.com/rastrea2r/rastrea2r) - Permite escanear discos e memória em busca de IOCs usando YARA no Windows, Linux e OS X.
* [Raccine](https://github.com/Neo23x0/Raccine) - Uma Proteção Simples contra Ransomware.
* [Stenographer](https://github.com/google/stenographer) - Solução de captura de pacotes que visa armazenar rapidamente todos os pacotes em disco.
* [sqhunter](https://github.com/0x4d31/sqhunter) - Caçador de ameaças baseado em osquery e Salt Open.
* [sysmon-config](https://github.com/SwiftOnSecurity/sysmon-config) - Template de arquivo de configuração do Sysmon com rastreamento de eventos de alta qualidade padrão.
* [sysmon-modular](https://github.com/olafhartong/sysmon-modular) - Um repositório de módulos de configuração do sysmon.
* [traceroute-circl](https://github.com/CIRCL/traceroute-circl) - Traceroute estendido para apoiar as atividades de operadores de CSIRT (ou CERT).

### Playbooks

* [AWS Incident Response Runbook Samples](https://github.com/aws-samples/aws-incident-response-runbooks) - Amostras de Runbook de IR da AWS destinadas a serem personalizadas por cada entidade que as utiliza.
* [Counteractive Playbooks](https://github.com/counteractive/incident-response-plan-template/tree/master/playbooks) - Coleção de Playbooks Counteractive.
* [GuardSIght Playbook Battle Cards](https://github.com/guardsight/gsvsoc_cirt-playbook-battle-cards) - Uma coleção de Cartas de Batalha de Playbook de Resposta a Incidentes Cibernéticos.
* [IRM](https://github.com/certsocietegenerale/IRM) - Metodologias de Resposta a Incidentes por CERT Societe Generale.
* [PagerDuty Incident Response Documentation](https://response.pagerduty.com/) - Documentos que descrevem partes do processo de Resposta a Incidentes da PagerDuty.
* [Phantom Community Playbooks](https://github.com/phantomcyber/playbooks) - Playbooks da Comunidade Phantom para Splunk, mas também personalizáveis para outros usos.
* [ThreatHunter-Playbook](https://github.com/OTRF/ThreatHunter-Playbook) - Playbook para auxiliar no desenvolvimento de técnicas e hipóteses para campanhas de caça.

### Ferramentas de Dump de Processos

* [Microsoft ProcDump](https://docs.microsoft.com/en-us/sysinternals/downloads/procdump) - Despeja qualquer imagem de memória de processos Win32 em execução em tempo real.
* [PMDump](http://www.ntsecurity.nu/toolbox/pmdump/) - Ferramenta que permite despejar o conteúdo da memória de um processo para um arquivo sem interromper o processo.

### Ferramentas de Sandbox/Engenharia Reversa

* [Any Run](https://app.any.run/) - Serviço interativo online de análise de malware para pesquisa dinâmica e estática.
* [CAPA](https://github.com/mandiant/capa) - Detecta capacidades em arquivos executáveis.
* [CAPEv2](https://github.com/kevoreilly/CAPEv2) - Malware Configuration And Payload Extraction.
* [Cutter](https://github.com/rizinorg/cutter) - Plataforma de Engenharia Reversa Gratuita e Open Source powered by rizin.
* [Ghidra](https://github.com/NationalSecurityAgency/ghidra) - Framework de Engenharia Reversa de Software.
* [Hybrid-Analysis](https://www.hybrid-analysis.com/) - Sandbox online poderoso e gratuito da CrowdStrike.
* [Intezer](https://analyze.intezer.com/#/) - Intezer Analyze mergulha em binários Windows para detectar similaridades de micro-código com ameaças conhecidas.
* [Joe Sandbox (Community)](https://www.joesandbox.com/) - Detecta e analisa arquivos e URLs potencialmente maliciosos em múltiplas plataformas.
* [Mastiff](https://github.com/KoreLogicSecurity/mastiff) - Framework de análise estática que automatiza a extração de características-chave de arquivos.
* [Metadefender Cloud](https://www.metadefender.com) - Plataforma gratuita de threat intelligence fornecendo multiscanning, sanitização de dados e avaliação de vulnerabilidades.
* [Radare2](https://github.com/radareorg/radare2) - Framework de engenharia reversa e conjunto de ferramentas de linha de comando.
* [Rizin](https://github.com/rizinorg/rizin) - Framework de engenharia reversa e conjunto de ferramentas de linha de comando UNIX-like.
* [StringSifter](https://github.com/fireeye/stringsifter) - Ferramenta de machine learning que classifica strings com base em sua relevância para análise de malware.
* [Threat.Zone](https://app.threat.zone) - Plataforma de análise de ameaças baseada em nuvem com sandbox, CDR e análise interativa.
* [Valkyrie Comodo](https://valkyrie.comodo.com) - Usa comportamento em tempo de execução e centenas de recursos de um arquivo para realizar análise.
* [Viper](https://github.com/viper-framework/viper) - Framework de análise e gerenciamento de binários baseado em Python.
* [Virustotal](https://www.virustotal.com) - Serviço online gratuito que analisa arquivos e URLs em busca de conteúdo malicioso.
* [Visualize_Logs](https://github.com/keithjjones/visualize_logs) - Biblioteca de visualização open source e ferramentas de linha de comando para logs.
* [Yomi](https://yomi.yoroi.company) - MultiSandbox gratuito gerenciado e hospedado pela Yoroi.

### Ferramentas de Scanner

* [Fenrir](https://github.com/Neo23x0/Fenrir) - Scanner IOC simples para sistemas Linux/Unix/OSX em bash puro.
* [LOKI](https://github.com/Neo23x0/Loki) - Scanner IR gratuito para escanear endpoint com regras yara e outros indicadores.
* [Spyre](https://github.com/spyre-project/spyre) - Scanner IOC simples baseado em YARA escrito em Go.

### Ferramentas de Linha do Tempo
* [Aurora Incident Response](https://github.com/cyb3rfox/Aurora-Incident-Response) - Plataforma desenvolvida para construir facilmente uma linha do tempo detalhada de um incidente.
* [Plaso](https://github.com/log2timeline/plaso) - Motor backend baseado em Python para a ferramenta log2tim

### Vídeos

* [The Future of Incident Response](https://www.youtube.com/watch?v=bDcx4UNpKNc) - Apresentado por Bruce Schneier no OWASP AppSecUSA 2015.
* [SIFT: Find Evil! Meeting AI Threat Speed with Defensive AI Orchestration](https://www.sans.org/presentations/keynote-sift-find-evil-meeting-ai-threat-speed-with-defensive-ai-orchestration) - Keynote de Rob T. Lee (SANS) no AI Cybersecurity Summit 2026 sobre orquestração de IA defensiva no SIFT Workstation[citation:9].
* [FIND EVIL! Hackathon: The Winners](https://www.sans.org/go/find-evil-hackathon-winners) - Apresentação dos vencedores do primeiro hackathon de resposta a incidentes autônoma da SANS, com análise dos harnesses vencedores[citation:16].

### Coleta de Evidências em Windows

* [AChoir](https://github.com/OMENScan/AChoir) - Framework/ferramenta de script para padronizar e simplificar a criação de utilitários de aquisição ao vivo para Windows.
* [Crowd Response](http://www.crowdstrike.com/community-tools/) - Aplicação de console Windows leve projetada para auxiliar na coleta de informações do sistema para resposta a incidentes.
* [DFIR ORC](https://dfir-orc.github.io/) - Coleção de ferramentas especializadas dedicadas a analisar e coletar artefatos críticos como MFT, hives de registro ou logs de eventos.
* [FastIR Collector](https://github.com/SekoiaLab/Fastir_Collector) - Coleta diferentes artefatos em sistemas Windows ao vivo e registra os resultados em arquivos csv.
* [Fibratus](https://github.com/rabbitstack/fibratus) - Ferramenta para exploração e rastreamento do kernel do Windows.
* [Hoarder](https://github.com/muteb/Hoarder) - Coleta os artefatos mais valiosos para investigações forenses ou de resposta a incidentes.
* [IREC](https://binalyze.com/products/irec-free/) - Coletor de Evidências de IR tudo-em-um que captura RAM Image, $MFT, EventLogs, WMI Scripts, Registry Hives e muito mais.
* [Invoke-LiveResponse](https://github.com/mgreen27/Invoke-LiveResponse) - Ferramenta de resposta ao vivo para coleta direcionada.
* [IRTriage](https://github.com/AJMartel/IRTriage) - Triagem de Resposta a Incidentes - Coleta de Evidências Windows para Análise Forense.
* [KAPE](https://www.kroll.com/en/services/cyber-risk/incident-response-litigation-support/kroll-artifact-parser-extractor-kape) - Kroll Artifact Parser and Extractor por Eric Zimmerman. Uma ferramenta de triagem que encontra os artefatos digitais mais prevalentes e os analisa rapidamente.
* [LOKI](https://github.com/Neo23x0/Loki) - Scanner IR gratuito para escanear endpoint com regras yara e outros indicadores (IOCs).
* [MEERKAT](https://github.com/TonyPhipps/Meerkat) - Triagem e caça a ameaças baseada em PowerShell para Windows.
* [Panorama](https://github.com/AlmCo/Panorama) - Visão geral rápida de incidentes em sistemas Windows ao vivo.
* [PowerForensics](https://github.com/Invoke-IR/PowerForensics) - Plataforma de forense de disco ao vivo, usando PowerShell.
* [PSRecon](https://github.com/gfoss/PSRecon/) - Coleta dados de um host Windows remoto usando PowerShell, organiza os dados em pastas, faz hash de todos os dados extraídos e os envia para a equipe de segurança.
* [RegRipper](https://github.com/keydet89/RegRipper3.0) - Ferramenta open source, escrita em Perl, para extrair/analisar informações (chaves, valores, dados) do Registro e apresentá-las para análise.

### 🤖 IA & LLM para IR

* [OSINT Forge Skills](https://github.com/OSINT-Forge-Community/osint-forge-skills) - 12 habilidades open-source de OSINT e forense digital para assistentes de IA (Claude Code, Codex, OpenCode, Gemini CLI). Investiga fontes, desafia hipóteses, analisa artefatos e produz relatórios referenciados com evidências preservadas e ferramentas Python offline[citation:1].
* [OGhidra](https://github.com/LLNL/OGhidra) - Ferramenta de análise binária impulsionada por IA que usa IAs agênticas hospedadas localmente para fazer engenharia reversa automática de binários para encontrar malware e vulnerabilidades. Suporta backends MCP (GhidraMCP) e PyGhidra para análise headless[citation:2][citation:19].
* [Reversecore MCP](https://github.com/sjkim1127/Reversecore_MCP) - Servidor MCP security-first que capacita agentes de IA a realizar engenharia reversa automatizada, análise de malware, forense digital e pesquisa de vulnerabilidades. Integra Radare2, r2ghidra, YARA, LIEF, Capstone, angr, Qiling e Volatility3 com prompts pré-construídos para análise de malware, ransomware triage, extração de C2 e mais[citation:3][citation:11].
* [Thorium](https://github.com/cisagov/thorium) - Plataforma automatizada e escalável de análise de malware e forense desenvolvida pela CISA e Sandia National Labs. Integra ferramentas comerciais, open-source e customizadas com workflows de análise automatizados. Capaz de processar mais de 10 milhões de ingestões de arquivos por hora por grupo de permissão e agendar mais de 1.700 jobs por segundo[citation:12].
* [Valhuntir](https://github.com/AppliedIR/sift-mcp) - Plataforma de resposta a incidentes aumentada por IA com SIFT MCP, gateway, portal do examinador e Valhuntir Lite. Fornece conhecimento forense RAG, banco de dados de triagem Windows, integração OpenCTI para threat intelligence e REMnux para análise automatizada de malware via MCP[citation:5][citation:13].
* [VERDICT](https://github.com/prabhakaran-jm/verdict) - Agente DFIR autônomo para SIFT que produz veredictos citados, auditados e offline-verificáveis. Usa um servidor MCP read-only que envolve Sleuth Kit, Volatility 3, YARA e EZ Tools; o modelo nunca recebe shell. Todas as descobertas devem citar `tool_call_id` + `output_sha256` + manifesto verificado. Submissão do SANS Find Evil! 2026[citation:6].
* [DFIR-AI](https://github.com/saivarun3407/DFIR-AI) - Agente de triagem DFIR autônomo e cross-OS com descobertas verificáveis, atestações assinadas e trilha de auditoria à prova de adulteração. Suporta múltiplos provedores de IA (Anthropic Claude, OpenAI, Ollama local para ambientes air-gapped) e mapeia descobertas para MITRE ATT&CK, NIST CSF 2.0 e ISO 27035[citation:7].
* [OATH (Verifier-Gated Evidence Receipts)](https://pypi.org/project/oath-mcp/) - Protótipo de pesquisa que separa o que um LLM propõe do que a evidência prova. Ferramentas forenses produzem envelopes `Notarized<T>` assinados, e o Witness Oath Verifier promove apenas alegações que podem ser deterministicamente re-derivadas dos bytes originais da evidência. Alcançou 92.75% TUS@4 em benchmark DFIR-Metric Module III com agente live + verifier[citation:17].

* [Aurora Incident Response](https://github.com/cyb3rfox/Aurora-Incident-Response) - Plataforma desenvolvida para construir facilmente uma linha do tempo detalhada de um incidente.
* [Plaso](https://github.com/log2timeline/plaso) - Motor backend baseado em Python para a ferramenta log2tim
