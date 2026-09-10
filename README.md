📋 Gestão de Ponto Técnico - Controle de Ocorrências e Divergências

Aplicação web responsiva desenvolvida para o gerenciamento, acompanhamento e registro de ocorrências de ponto para equipes técnicas de campo. O sistema oferece controle individualizado por colaborador, atalhos para motivos frequentes de divergência (fora da cerca, falha de app, bateria, esquecimento), relatórios mensais consolidados e capacidade de impressão.

✨ Principais Recursos

👥 Gestão de Colaboradores (CRUD):

Adição de novos técnicos.

Edição de nome e cargo/função.

Exclusão com confirmação e remoção em cascata dos históricos associados.

Ordenação automática e permanente por ordem alfabética.

📍 Registro de Ocorrências e Divergências:

Classificação de situação (Ponto Normal dentro da cerca, Ponto registrado fora da cerca, Justificado divergência de horário).

Atalhos rápidos para preenchimento de justificativas comuns:

📶 Falha no app/conexão

🔋 Técnico avisou que acabou bateria do celular

⏰ Técnico avisou que acabou esquecendo de registrar o ponto

Campo obrigatório de detalhamento/observação.

📅 Filtros e Relatórios Mensais:

Filtro global por mês (YYYY-MM) e busca textual por nome de técnico ou cargo.

Modal dedicado para Relatório Mensal, agrupando todas as ocorrências de um mês específico por colaborador.

Indicadores dinâmicos (Total de Técnicos e Total de Ocorrências por Período).

🖨️ Impressão e Exportação para PDF:

Estilização dedicada para impressão (@media print), ocultando menus, modais e elementos visuais de sistema, exibindo uma tabela limpa e legível.

Opção de impressão rápida tanto do relatório geral quanto do relatório mensal consolidado.

💾 Armazenamento Local e Persistência:

Salva automaticamente as alterações e registros no navegador do usuário via localStorage.

Inicialização automática com a lista padrão de 21 técnicos responsáveis.

🎨 Design Moderno em Dark Mode:

Interface escura de alto contraste com detalhes na cor Vermelho / Brand Red.

Notificações estilo Toast dinâmicas.

👷 Listagem de Técnicos Pré-Cadastrados (21 Colaboradores)

O sistema é iniciado automaticamente com os seguintes técnicos em ordem alfabética:

Alessandro Pires

Bruno Severes

Cleverson Polazzo

Ederson Carvalho

Edson Rocker

Guilherme Stujk

Kauan Miranda

Leonardo Longo

Marcio Ribeiro

Marcos Brandalize

Mateus Mattos

Odair Antunes

Renan Fagundes

Renan Tartari

Rodrigo Boff

Samuel Martins

Serginho Brugalli

Tiago Negri

Valdenor Sotoriva

Vinicios Candatten

Wellinton de Liz

🛠️ Tecnologias Utilizadas

HTML5: Estrutura semântica e acessível.

Tailwind CSS v3 (CDN): Estilização moderna e utilitária com suporte nativo a temas escuros.

JavaScript (ES6+): Lógica da aplicação, manipulação do DOM e gerenciamento do localStorage.

FontAwesome 6: Ícones vetoriais em toda a interface.

Google Fonts (Inter): Tipografia clara e legível.

🚀 Como Executar o Projeto

Faça o download ou copie o arquivo registro_ponto.html.

Abra o arquivo em qualquer navegador web moderno (Google Chrome, Microsoft Edge, Firefox, Safari).

Não é necessário instalar nenhuma dependência de servidor ou backend (aplicação 100% Client-Side).

📖 Guia de Utilização

1. Registrar uma Ocorrência

Na linha do técnico desejado na tabela, clique no botão vermelho "Ocorrência" (ou use a opção rápida).

Selecione a Data da ocorrência.

Escolha a Situação/Tipo:

✅ Ponto Normal dentro da cerca

📍 Ponto registrado fora da cerca

⚠️ Justificado divergência de horário

Utilize os Atalhos de Motivos Frequentes ou digite a observação no campo de texto.

Clique em "Salvar Registro".

2. Consultar o Histórico de um Técnico

Clique no ícone de relógio (Histórico) na coluna de ações da linha do colaborador.

Visualize todas as ocorrências salvas em ordem cronológica.

Se necessário, exclua uma ocorrência específica utilizando o ícone de lixeira.

3. Visualizar e Imprimir o Relatório Mensal

Clique no botão "Relatório Mensal" no topo da página.

Selecione o mês/ano desejado no filtro.

Visualize os colaboradores que possuem ocorrências naquele mês.

Clique em "Imprimir Este Mês" ou utilize Ctrl + P para gerar um documento PDF/impresso formatado.

4. Gerenciar Colaboradores

Novo Colaborador: Clique no botão "Novo Colaborador" no topo para adicionar um técnico à lista.

Editar: Clique no ícone de lápis na linha do técnico para renomeá-lo ou alterar a função.

Excluir: Clique no ícone de lixeira vermelha para remover o técnico (atenção: excluir um técnico também remove o histórico associado).

🔒 Armazenamento de Dados

A aplicação utiliza as seguintes chaves no localStorage do navegador:

gestao_ponto_techs: Armazena o array de objetos dos colaboradores cadastrados.

gestao_ponto_records: Armazena o histórico completo de ocorrências de ponto lançadas.

Nota: Por usar armazenamento local do navegador, os dados salvos ficam restritos ao navegador/computador em que foram lançados. Para backup ou troca de computador, recomenda-se a impressão dos relatórios mensais em formato PDF.
