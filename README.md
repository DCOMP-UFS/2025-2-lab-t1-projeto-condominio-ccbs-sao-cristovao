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
* **Grupos Integrados e Acessos:**

    * **GESEC (Gênero, Sexualidade e Estudos Culturais):** Vinculado ao departamento de Psicologia, o projeto foca em dar suporte tecnológico às investigações em Ciências Humanas, garantindo segurança para dados sensíveis.
        * 🔗 **Acesso:** [http://18.208.246.100](http://18.208.246.100)

    * **GEPESCEF (Grupo de Estudos e Pesquisas Sociedade, Cultura e Educação Física):** Investiga as interfaces entre esporte, saúde, cultura e sociedade. O portal centraliza seus projetos de pesquisa (PIAs) e produção científica.
        * 🔗 **Acesso:** [http://3.236.42.58](http://3.236.42.58)

    * **Laboratório de Odontologia:** Infraestrutura voltada para o suporte tecnológico ao ensino e pesquisa odontológica, focando na gestão eficiente de recursos computacionais e confiabilidade de dados.
        * 🔗 **Acesso:** [http://18.204.231.5](http://18.204.231.5)

    * **Formação e Atuação Docente:** Grupo dedicado a estudos sobre educação, práticas pedagógicas, corporeidade e políticas educacionais, visando a formação continuada de professores.
        * 🔗 **Acesso:** [http://52.4.95.25](http://52.4.95.25)

    * **DOM (Dor e Motricidade):** Vinculado ao Departamento de Fisioterapia, estuda mecanismos de dor e efeitos terapêuticos de intervenções não farmacológicas.
        * 🔗 **Acesso:** *(Em breve)*

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

## 🌐 Acesso ao Projeto Principal

O portal central do Condomínio CCBS (integrador) está implantado e acessível publicamente através da infraestrutura da AWS Academy.

🔗 **Acesse o Portal Integrador:** [http://98.81.160.226/#infraestrutura](http://98.81.160.226/#infraestrutura)

---

**Equipe Técnica:**
* Cauan Teixeira Machado
* José Gabriel Remigio Gama de Almeida
* Carlos Gabriel Dias Fontes
* José Weverton de Oliveira Vilar
* Joseph Antony dos Santos Leite

**Supervisão Docente:**
* Profa. Edilayne Meneses
