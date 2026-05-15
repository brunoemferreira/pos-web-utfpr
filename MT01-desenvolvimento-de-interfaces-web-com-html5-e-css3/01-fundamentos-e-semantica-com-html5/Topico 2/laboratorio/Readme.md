# 🛠️ Laboratório 2: Formulário de Cadastro Inteligente

Nesta atividade, você construirá um formulário de inscrição para um evento técnico. O desafio é garantir que o navegador valide todas as regras de negócio sem que você precise escrever nenhum código JavaScript. Imagine que você está criando a página de inscrição para a **"UTFPR Tech Week"**. O formulário precisa ser amigável para quem usa celular e rígido com os dados inseridos para evitar cadastros falsos.

---

### 📋 Tarefas

#### Tarefa 1: Estrutura e Acessibilidade
- Crie o arquivo `cadastro.html`.
- Utilize `<fieldset>` e `<legend>` para agrupar as informações (ex: "Dados Pessoais" e "Preferências do Evento").
- **Regra de Ouro:** Cada campo de entrada deve ter um `<label>` explicitamente vinculado a ele usando o atributo `for`.

#### Tarefa 2: Implementação de Tipos e Validações
Crie os seguintes campos aplicando as restrições solicitadas:
- **Nome Completo:** Texto, obrigatório, mínimo de 5 caracteres.
- **E-mail:** Tipo `email`, obrigatório.
- **Data de Nascimento:** Tipo `date`, obrigatório (Dica: tente limitar a data máxima para hoje).
- **Quantidade de Convidados:** Tipo `number`, mínimo 0 e máximo 5.
- **URL do Portfólio:** Tipo `url`, não obrigatório, mas se preenchido, deve ser um link válido.
- **Senha:** Tipo `password`, obrigatório, mínimo de 8 caracteres.
- **Nível de Experiência:** Um seletor do tipo `range` de 1 a 10.

#### Tarefa 3: O Desafio do Pattern
- Crie um campo para **Telefone** (`type="tel"`).
- Pesquise ou utilize a IA para criar um atributo `pattern` que aceite apenas o formato brasileiro com DDD: `(XX) XXXXX-XXXX`.
- Adicione o atributo `title` para explicar ao usuário o formato esperado caso ele erre.

---

### 🔍 Como testar seu laboratório?
1. Abra o arquivo no navegador.
2. Tente clicar no botão de **"Enviar"** com o formulário vazio.
3. Tente inserir um e-mail sem o `@` ou um número de convidados maior que 5.
4. **O sucesso é atingido** quando o navegador bloqueia o envio e exibe um alerta nativo em cada um desses erros.
