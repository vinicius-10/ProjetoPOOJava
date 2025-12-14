# 📚 Sistema de Controle de Acervo Bibliográfico

> Projeto desenvolvido para a disciplina de Programação Orientada a Objetos (POO).

![Language](https://img.shields.io/badge/Linguagem-C-orange)
![Status do Projeto](https://img.shields.io/badge/Status-Concluído-green)
![Tipo](https://img.shields.io/badge/Tipo-Acadêmico-blue)

## 📖 Sobre o Projeto

Este sistema é uma aplicação para o gerenciamento interno do acervo de uma biblioteca. O objetivo principal foi aplicar conceitos sólidos de POO na criação de um software capaz de gerenciar autores, editoras e diferentes tipos de livros, garantindo a integridade dos dados e regras de negócio específicas.

O projeto passou por uma refatoração significativa, migrando de uma interface baseada em console (Menus/Leitura) para uma Interface Gráfica baseada em Formulários (**Forms**), melhorando a usabilidade e a experiência do usuário.

## 🚀 Funcionalidades

### 👥 Gerenciamento de Autores e Editoras
O sistema permite o controle completo de quem produz as obras:
* **Cadastro:** Inserção de novos autores e editoras.
* **Listagem:** Visualização de todos os cadastrados em lista.
* **Busca Específica:** Localização rápida via **CPF** (Autores) ou **CNPJ** (Editoras).
* **Edição com Travas:** Atualização de dados cadastrais e status (Disponível/Indisponível). *Nota: Campos chave como CPF e CNPJ são imutáveis após o cadastro.*
* **Bloqueio/Desbloqueio:** Permite bloquear autores ou editoras, impedindo que sejam associados a novos livros temporariamente.

### 📚 Gerenciamento de Livros
O sistema suporta três categorias de obras, com regras específicas para cada uma:
1.  **Didático**
2.  **Infantil**
3.  **Colecionável**

**Destaques do módulo de livros:**
* **Cadastro Centralizado:** Formulário único inteligente. Ao selecionar o tipo do livro, o sistema exibe apenas os campos específicos daquela categoria.
* **Identificação Polimórfica:** O sistema permite IDs iguais para livros de *tipos diferentes* (ex: O livro ID 1 do tipo Infantil é diferente do livro ID 1 do tipo Didático).
* **Atualização:** Edição de dados do livro e status de ativação/desativação. *Nota: ID e Tipo do livro não podem ser alterados.*

### 🔍 Busca Avançada e Visualização
* **Tabela Unificada:** Exibição de todos os tipos de livros em uma única tabela.
* **Filtro em Tempo Real:** Filtragem dinâmica digitando partes do **Título**, **Nome da Editora** ou **Nome do Autor**.
* **Detalhamento:** Ao clicar em um item da tabela, todas as informações detalhadas da obra são exibidas.

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** [Insira a linguagem, ex: Java, C#, Python]
* **Interface Gráfica:** [Insira a lib gráfica, ex: Java Swing, JavaFX, Windows Forms]
* **Persistência de Dados:** [Ex: Arquivos, Banco de dados MySQL, H2, Lista em Memória]
* **IDE:** [Ex: Eclipse, IntelliJ, Visual Studio]

## 🧩 Conceitos de POO Aplicados

Durante o desenvolvimento, foram utilizados os seguintes pilares da orientação a objetos:

* **Herança:** Utilizada para compartilhar atributos comuns entre os diferentes tipos de Livros.
* **Polimorfismo:** Permite tratar `LivroDidatico`, `LivroInfantil` e `LivroColecionavel` de forma genérica nas listagens e buscas.
* **Encapsulamento:** Proteção dos dados sensíveis (como IDs e Documentos) através de métodos de acesso e restrições de edição nos Forms.

---

## 🔧 Como Executar

1. Clone o repositório:
   ```bash
   git clone [https://github.com/seu-usuario/nome-do-repo.git](https://github.com/seu-usuario/nome-do-repo.git)

2. Abra o projeto na sua IDE de preferência.

3. Certifique ter pelo menos o JDK 20 instalado

4. Execute a classe principal Main.

✒️ Autor
Vinicius Souza Dias - Desenvolvimento e Refatoração
