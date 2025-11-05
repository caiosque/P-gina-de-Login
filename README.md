# 🔐 Sistema de Login Simples

Um projeto front-end desenvolvido com **HTML, CSS e JavaScript puro**,
simulando um sistema de login com páginas complementares de
**recuperação de senha** e **sobre mim**.\
Ideal para portfólios, práticas de layout responsivo e introdução à
estrutura de aplicações web estáticas.

------------------------------------------------------------------------

## 📂 Estrutura do Projeto

    📁 Projeto-Login/
    ├── login.html         # Página principal de login
    ├── recuperar.html     # Página para recuperação de senha
    ├── sobre.html         # Página de informações sobre o autor
    └── style.css          # Arquivo de estilos globais

------------------------------------------------------------------------

## 🖥️ Páginas do Projeto

### **1. Página de Login (`login.html`)**

-   Contém um formulário para entrada de usuário e senha.\
-   Inclui botão de alternância ("Mostrar/Ocultar senha") com
    JavaScript.\
-   Links de navegação para **recuperar senha** e **sobre mim**.\
-   Layout centralizado e responsivo.

**Funcionalidades principais:** - Campos com *autocomplete*. - Validação
básica via HTML (`type="password"`, `type="text"`). - Função JavaScript
`toggleSenha()` que altera dinamicamente o tipo do campo de senha.

------------------------------------------------------------------------

### **2. Página de Recuperação de Senha (`recuperar.html`)**

-   Permite ao usuário inserir o e-mail cadastrado.\
-   Exibe uma mensagem de confirmação simulando o envio de instruções.\
-   Inclui link para retornar à tela de login.

**Função JavaScript:**

``` js
function enviarEmail() {
  const email = document.getElementById('email').value;
  const msg = document.getElementById('mensagem');
  if (email.trim() === "") {
    msg.textContent = "Por favor, preencha seu e-mail.";
  } else {
    msg.textContent = "Se o e-mail estiver cadastrado, enviaremos as instruções de recuperação.";
  }
}
```

------------------------------------------------------------------------

### **3. Página Sobre Mim (`sobre.html`)**

-   Página com texto descritivo genérico e espaço para informações
    pessoais/profissionais.\
-   Ideal para personalização --- substitua os textos pelo seu perfil
    real.\
-   Inclui links de contato e navegação entre as outras páginas.

------------------------------------------------------------------------

## 🎨 Estilo e Design (`style.css`)

O arquivo de estilos define um visual moderno e responsivo:

-   **Paleta de cores:** tons de azul e branco translúcido, com
    gradiente suave.\
-   **Layout:** centrado verticalmente, com uso de `flexbox`.\
-   **Componentes:** botões com sombra e bordas arredondadas, cartões de
    conteúdo (`.card`), rodapé fixo com leve desfoque.\
-   **Responsividade:** ajustes automáticos de fonte e espaçamento em
    telas menores.

Exemplo de estrutura base:

``` css
.card {
  background: rgba(255,255,255,0.92);
  border-radius: 12px;
  box-shadow: 0 8px 24px rgba(4,24,48,0.25);
}
```

------------------------------------------------------------------------

## ⚙️ Como Executar

1.  **Baixe ou clone o repositório:**

    ``` bash
    git clone https://github.com/seuusuario/projeto-login.git
    ```

2.  **Abra o arquivo principal no navegador:**

    ``` bash
    cd projeto-login
    start login.html   # (Windows)
    # ou
    open login.html    # (macOS/Linux)
    ```

3.  **Navegue entre as páginas** pelos links no rodapé ou nos botões de
    ação.

------------------------------------------------------------------------

## 📱 Responsividade

O layout foi projetado para se ajustar automaticamente em diferentes
resoluções.\
Em dispositivos móveis, os cartões diminuem o espaçamento e a tipografia
se adapta para melhor leitura.

------------------------------------------------------------------------

## 💡 Possíveis Extensões Futuras

-   Conexão com backend (Node.js, Python ou PHP).
-   Validação real de login e recuperação de senha.
-   Tema escuro (Dark Mode).
-   Animações de transição entre páginas.

------------------------------------------------------------------------

## 🧑‍💻 Autor

**Caio Samuel Carvalho do Nascimento**\
Estudante de **Licenciatura em Computação**, apaixonado por
desenvolvimento web e interfaces acessíveis.

📧 <caio.samuel.c.n@gmail.com>\
🌐 Projeto feito com dedicação para fins de aprendizado e portfólio.

------------------------------------------------------------------------

## 📝 Licença

Este projeto é distribuído sob a licença **MIT**, o que significa que
você pode usar, modificar e distribuir livremente, desde que mantenha os
créditos ao autor original.

------------------------------------------------------------------------
