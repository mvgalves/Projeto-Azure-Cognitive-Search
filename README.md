# 🔍 Azure Cognitive Search: Utilizando AI Search para Indexação e Consulta de Dados

## 📘 Descrição do Projeto

Este projeto foi desenvolvido como parte do laboratório prático da DIO, com foco na aplicação de técnicas de ingestão de dados, criação de índices inteligentes e uso de buscas cognitivas utilizando os serviços oferecidos pela plataforma Azure, em especial o **Azure Cognitive Search**.

A proposta do laboratório é aplicar conhecimentos teóricos adquiridos durante as aulas em um ambiente prático, explorando a capacidade da inteligência artificial para organizar, enriquecer e pesquisar grandes volumes de dados de forma eficiente.

---

## 🎯 Objetivos

- Aplicar a ingestão de dados por meio de fontes como Blob Storage, Data Lake Storage e Table Storage;
- Enriquecer dados com habilidades cognitivas (AI enrichment) como OCR, extração de entidades, idioma e chave-conceito;
- Criar e configurar índices de busca inteligentes;
- Realizar consultas e navegação com suporte à linguagem natural;
- Documentar o processo técnico com clareza para fins de aprendizado e reprodutibilidade.

---

## 🧰 Tecnologias e Serviços Utilizados

- [Azure Cognitive Search](https://learn.microsoft.com/azure/search/)
- [Azure Blob Storage](https://learn.microsoft.com/azure/storage/blobs/)
- [Azure Data Lake Storage](https://learn.microsoft.com/azure/storage/data-lake-storage/)
- [Azure Table Storage](https://learn.microsoft.com/azure/storage/tables/table-storage-overview)
- Azure Cognitive Services (OCR, Key Phrases, Entity Recognition)
- Portal Azure + Interface de Configuração de Indexadores
- GitHub (para versionamento e documentação)

---

## 🗂️ Estrutura do Projeto  


azure-ai-search-lab/  
│   
└── README.md # Documentação do projeto  

---

## 🚀 Etapas Realizadas

### 1. Ingestão de Dados
- Arquivos reais (.pdf, .txt e .json) foram armazenados em um **Azure Blob Storage**.
- Uma conexão foi configurada entre o serviço de armazenamento e o Azure Cognitive Search por meio de um **Data Source**.

### 2. Enriquecimento com IA
- Adicionado um **Skillset Cognitivo** ao pipeline de indexação.
- Aplicadas habilidades como:
  - Extração de texto por OCR
  - Identificação de linguagem
  - Extração de entidades e frases-chave

### 3. Criação do Índice
- Definido esquema de índice com campos como `title`, `content`, `language`, `keyPhrases`, `entities`.
- Utilizado `semantic search` para melhoria na interpretação da consulta.

### 4. Indexador
- Criado indexador para processar os dados e alimentar o índice automaticamente.
- Agendamento configurado para manter o índice atualizado.

### 5. Consultas Cognitivas
- Realizadas buscas com suporte a linguagem natural como:
  - "Quais serviços de IA existem no Azure?"
  - "Resuma os principais recursos do Blob Storage"
- Resultados apresentaram respostas enriquecidas com contexto, entidades e pontuação semântica.

---

## ✅ Resultados Obtidos

- Dados foram enriquecidos com sucesso, identificando entidades como nomes próprios, localizações e palavras-chave.
- O índice cognitivo permitiu buscas semânticas precisas, retornando resultados com base em relevância contextual.
- A arquitetura mostrou-se escalável e reutilizável para outros tipos de dados (imagens, planilhas, etc).

---

## 🧠 Aprendizados

- Domínio prático do pipeline de ingestão e indexação no Azure Cognitive Search
- Compreensão do fluxo entre armazenamento -> enriquecimento -> indexação -> consulta
- Fortalecimento das práticas de documentação técnica com uso do GitHub

---

## 📌 Conclusão

Este projeto demonstrou na prática o poder do **Azure Cognitive Search** na transformação de dados brutos em informações pesquisáveis com inteligência artificial. A integração entre os serviços Azure mostra-se altamente eficaz para aplicações que demandam recuperação de informação baseada em contexto, linguagem natural e alto volume de dados.

---

## 🔗 Referências

- [Microsoft Learn - Explore an Azure AI Search index (UI)](https://learn.microsoft.com/en-us/training/modules/explore-azure-ai-search-index/)
- [Documentação Oficial do Azure Cognitive Search](https://learn.microsoft.com/en-us/azure/search/)
- [DIO - Formação Azure AI Fundamentals](https://www.dio.me)
