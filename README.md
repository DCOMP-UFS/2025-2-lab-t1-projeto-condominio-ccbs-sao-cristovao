# Projeto de Infraestrutura de Redes: Condomínio CCBS - UFS

> **Disciplina:** Laboratório de Redes de Computadores (2025.2)  
> **Departamento:** Computação (DCOMP) - Universidade Federal de Sergipe (UFS)  

## 📌 Visão Geral

Este repositório documenta o planejamento e a implementação simulada da infraestrutura de redes para o **Centro de Ciências Biológicas e da Saúde (CCBS)**. O projeto adota o modelo de "Condomínio de Laboratórios", visando a integração lógica e física de diversos grupos de pesquisa e departamentos (Odontologia, Fisioterapia, Psicologia e Educação Física) sob uma infraestrutura unificada, segura e de alto desempenho.

O projeto abrange desde a modelagem física na planta baixa até a viabilidade financeira baseada em pregões reais, culminando na implementação de um portal de serviços hospedado em nuvem.

## 🚀 Escopo do Projeto

O desenvolvimento foi estruturado em três pilares principais:

1.  **Modelagem e Topologia:** Planejamento do cabeamento estruturado, definição de VLANs para segmentação de tráfego (Pesquisa, Administrativo, Visitante) e posicionamento estratégico de Access Points (APs).
2.  **Orçamento Realista:** Levantamento de custos de hardware (Switches L2/L3, Roteadores, Servidores e Workstations) baseado estritamente em **Atas de Licitação** vigentes, garantindo conformidade com a realidade do setor público.
3.  **Implementação de Serviços (Web):** Desenvolvimento e *deploy* de uma aplicação web para centralizar as informações dos grupos de pesquisa, hospedada em uma instância **EC2 na AWS Academy**.

## 📂 Estrutura do Repositório

Abaixo segue a descrição técnica dos principais arquivos e entregáveis deste projeto:

### `index.html` (Portal do Condomínio CCBS)
Código-fonte da interface web hospedada na AWS. Trata-se de uma *Single Page Application* (SPA) leve, desenvolvida com **HTML5, CSS3 e Vanilla JavaScript**, sem dependência de frameworks pesados.
* **Funcionalidade:** Utiliza manipulação de DOM para alternar dinamicamente entre as subpáginas dos grupos de pesquisa sem recarregamento da página.
* **Design:** Implementa um design responsivo e uma paleta de cores institucional (baseada no padrão azul/branco da UFS e CCBS), utilizando variáveis CSS (`:root`) para fácil manutenção.
* **Grupos Integrados:**
    * **GESEC:** Gênero, Sexualidade e Estudos Culturais (Psicologia).
    * **DOM:** Grupo de Pesquisa Dor e Motricidade (Fisioterapia).
    * **GEPESCEF:** Grupo de Estudos e Pesquisas Sociedade, Cultura e Educação Física.
    * **Laboratório de Odontologia.**
    * **Grupo de Pesquisa Formação e Atuação Docente.**

### `lista-de-dispositivos.md` (Inventário de Hardware)
Documento técnico contendo o levantamento quantitativo e as especificações dos ativos de rede e equipamentos terminais orçados.
* **Core da Rede:** Switch H3C S5170-54S-EI (48 portas + 10GB SFP+) e Roteadores OMADA com suporte a VPN/VLAN.
* **Conectividade Wireless:** Access Points Ubiquiti UniFi U6+ Pro (Wi-Fi 6) para alta densidade.
* **Terminais e Energia:** Workstations All-in-one, Notebooks de alto desempenho (Core i5-12450HX) e sistema de proteção elétrica (Nobreaks 1500VA).
* **Infraestrutura Passiva:** Cabeamento CAT6A para suportar tráfego 10GbE no backbone.

## 🛠️ Tecnologias e Ferramentas

* **Infraestrutura de Nuvem:** AWS EC2 (Amazon Linux/Ubuntu).
* **Web Server:** Apache/Nginx (Configuração de servidor web).
* **Front-end:** HTML5, CSS3 (Grid/Flexbox), JavaScript.
* **Hardware de Referência:** H3C, Ubiquiti, Lenovo, TP-Link (Omada).

## 🌐 Acesso ao Projeto

O portal do Condomínio CCBS está implantado e acessível publicamente através da infraestrutura da AWS Academy.

🔗 **Acesse aqui:** http://98.81.160.226/#infraestrutura

---

**Equipe Técnica:**
* Cauan Teixeira Machado
* José Gabriel Remigio Gama de Almeida
* Carlos Gabriel Dias Fontes
* José Weverton de Oliveira Vilar
* Joseph Antony dos Santos Leite

**Supervisão Docente:**
* Profa. Edilayne Meneses
