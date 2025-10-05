Nome do Projeto: Shark Sentinel
(Um bom nome é memorável. "Sentinela dos Tubarões" soa protetor e tecnológico.)

Slogan: Usando dados da NASA para prever e proteger os habitats de tubarões contra a pesca predatória.

1. Contexto do Projeto e o Problema (Problem Statement)
A pesca acidental, ou "bycatch", é uma das maiores ameaças às populações de tubarões em todo o mundo. Frotas de pesca comercial, ao buscarem outras espécies, frequentemente operam em áreas que também servem como zonas de alimentação e migração para tubarões, resultando em capturas não intencionais que dizimam espécies vulneráveis. O problema central é que esses habitats marinhos são dinâmicos e se movem com as correntes e a disponibilidade de alimento, tornando difícil para as autoridades e para a própria indústria pesqueira evitar essas sobreposições fatais.

2. Nossa Solução: A Plataforma Shark Sentinel
O Shark Sentinel é uma plataforma de mapeamento preditivo baseada na web, projetada para analisar dados de satélite da NASA em tempo quase real. Nossa ferramenta processa múltiplas camadas de informações oceanográficas — como concentração de clorofila-a (indicador de fitoplâncton), temperatura da superfície do mar e padrões de correntes marítimas — para identificar áreas com alta probabilidade de serem zonas de forrageamento (alimentação) de tubarões. Ao cruzar essas previsões com dados de rastreamento de frotas pesqueiras (AIS), a plataforma gera um mapa de risco, destacando "hotspots" onde o perigo de bycatch é mais elevado, permitindo uma ação preventiva.

3. Público-Alvo
Nosso projeto é direcionado a três grupos principais que podem utilizar nossa ferramenta para tomar decisões mais informadas:

ONGs de Conservação Marinha: Para direcionar campanhas de conscientização, fiscalização e lobby por áreas de proteção marinha.

Agências Governamentais de Pesca e Meio Ambiente: Para planejar rotas de pesca mais sustentáveis, definir zonas de exclusão temporárias e fiscalizar a atividade pesqueira de forma mais eficiente.

Pesquisadores e Biólogos Marinhos: Para estudar a ecologia dos tubarões, entender seus padrões de movimento e aprofundar o conhecimento sobre suas interações com atividades humanas.

4. Funcionalidades Principais (Features)
Mapa Interativo: Uma interface de mapa global onde os usuários podem visualizar as camadas de dados de forma intuitiva.

Heatmap Preditivo de Habitat: A principal funcionalidade da plataforma, exibindo as áreas de maior probabilidade de atividade de tubarões com base em nosso modelo.

Filtros de Dados e Linha do Tempo: Os usuários poderão filtrar dados por espécie (inicialmente focado no Tubarão Branco), período de tempo e visualizar a evolução dos habitats ao longo das semanas.

Camada de Risco de Bycatch: Sobreposição dos hotspots de tubarões com as rotas comuns de pesca para gerar um índice de risco visual (verde, amarelo, vermelho).

5. Pipeline de Dados e Pilha Tecnológica (Tech Stack)
Fontes de Dados:

NASA MODIS Aqua/Terra: Para dados de concentração de Clorofila-a.

NASA PO.DAAC: Para dados de temperatura da superfície do mar e vetores de correntes oceânicas.

Global Fishing Watch: Para dados de rastreamento de embarcações de pesca (AIS).

Backend: Python com as bibliotecas Pandas, GeoPandas e Scikit-learn para processamento e análise dos dados. A API será construída com FastAPI pela sua alta performance.

Frontend: React.js com TypeScript para uma interface robusta e interativa.

Visualização de Mapas: Mapbox ou Leaflet.js para renderizar os mapas e as camadas de dados.

Banco de Dados: PostgreSQL com a extensão PostGIS para armazenar e consultar dados geoespaciais de forma eficiente.

6. Estrutura de Arquivos do Projeto
Uma estrutura de monorepositório para facilitar o desenvolvimento:

/shark-sentinel
|
|-- /backend                # Código da API e processamento de dados (Python)
|   |-- /scripts            # Scripts para baixar e processar dados da NASA
|   |-- main.py             # Arquivo principal da API
|   `-- requirements.txt      # Dependências do Python
|
|-- /frontend               # Código da interface web (React)
|   |-- /public
|   |-- /src                # Componentes React, estilos, etc.
|   `-- package.json        # Dependências do JavaScript
|
|-- .gitignore              # Arquivos a serem ignorados pelo Git
`-- README.md               # Este arquivo de apresentação
7. Produto Mínimo Viável (MVP) para o Hackathon
Dado o tempo limitado, nosso foco é entregar um protótipo funcional que prove nosso conceito:

Coletar e processar dados de uma única região geográfica (ex: Costa da Califórnia).

Implementar o modelo preditivo básico para gerar um heatmap de habitat para uma única espécie.

Exibir este heatmap em um mapa interativo simples no frontend.

A atualização dos dados será manual para a demonstração.

8. Próximos Passos e Futuro do Projeto
Expandir a cobertura para uma escala global.

Integrar modelos de Machine Learning para aprimorar a acurácia das previsões.

Adicionar mais espécies de tubarões e outras espécies marinhas ameaçadas.

Desenvolver um sistema de alertas em tempo real para as autoridades quando uma embarcação de pesca entrar em uma zona de alto risco.

9. Equipe
Caio 
Rafael
Eduardo
Henrique
Bruno
Erick




