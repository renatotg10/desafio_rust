# Desafio 21 Dias de Rust
##### 25/03/2024 - Professor: Danilo Aparecido do Torne-se um Programador
##### https://www.torneseumprogramador.com.br/
---

## Instalação do Rust

Aqui estão as instruções básicas para instalar o Rust nos sistemas operacionais Windows, Linux e MacOS:

### Windows:

1. **Baixe e instale o Visual Studio com as Ferramentas C++:**
   Acesse [o site oficial do Visual Studio](https://visualstudio.microsoft.com/pt-br/downloads) e clique no botão "Download gratuito". Isso irá baixar um arquivo executável (.exe) que instalará o Visual Studio no seu sistema. Para utilizar o Rust no Windows é necessário instalar a IDE **Visual Studio** da Microsoft com as ferramentas para compilação C++.

2. **Baixe o instalador do Rust:**
   Acesse [o site oficial do Rust](https://www.rust-lang.org/tools/install) e clique no botão "Download Rustup". Isso irá baixar um arquivo executável (.exe) que instalará o Rust e o Cargo (gerenciador de pacotes) no seu sistema.

3. **Execute o instalador:**
   Dê um duplo clique no arquivo .exe baixado e siga as instruções na tela para completar a instalação.

4. **Verifique a instalação:**
   Abra um terminal (pode ser o CMD ou PowerShell) e digite:
   ```bash
   rustc --version
   ```
   Isso deve exibir a versão do Rust instalada.

### Linux e MacOS:

1. **Instale o Rust usando `rustup`:**
   Abra um terminal e execute o seguinte comando:
   ```bash
   curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
   ```
   Isso baixará e executará o script de instalação do `rustup`, que é um gerenciador de versões do Rust.

2. **Siga as instruções na tela:**
   O script de instalação irá pedir que você pressione `Enter` para iniciar a instalação. Em seguida, siga as instruções na tela para completar a instalação.

3. **Verifique a instalação:**
   Após instalar e configurar, você pode verificar se o Rust foi instalado corretamente digitando no terminal:
   ```bash
   rustc --version
   ```
   Isso deve exibir a versão do Rust instalada.

4. **No caso do instalador não ter adicionado o Rust ao PATH, faça isso manualmente:**
   No final da instalação, o `rustup` irá instruí-lo a adicionar o diretório bin do Rust ao seu PATH. Siga as instruções para fazer isso. Se você não as viu ou as ignorou, você pode fazer isso manualmente adicionando a seguinte linha ao seu arquivo de configuração do shell (como `.bashrc`, `.bash_profile`, `.zshrc`, etc.):
   ```bash
   export PATH="$HOME/.cargo/bin:$PATH"
   ```
   Depois de adicionar isso, reinicie o terminal ou execute `source ~/.bashrc` (ou o arquivo de configuração do seu shell) para atualizar as configurações.

## Olá, mundo!

Documentação do Rust pode ser encontrada no site https://rust-br.github.io/rust-book-pt-br/.

Para criar um programa "Hello, World!" em Rust, siga estes passos simples:

1. **Crie um novo projeto:**
   Abra um terminal e navegue até o diretório onde deseja criar seu projeto. Em seguida, execute o seguinte comando para criar um novo projeto Rust usando Cargo (o gerenciador de pacotes do Rust):
   ```bash
   cargo new hello_world
   ```
   Isso criará um novo diretório chamado `hello_world` com uma estrutura básica de projeto Rust.

3. **Edite o arquivo fonte:**
   Navegue para o diretório do seu projeto recém-criado:
   ```bash
   cd hello_world
   ```
   Abra o arquivo `src/main.rs` em um editor de texto. Este arquivo contém o código fonte do seu programa Rust.

4. **Escreva o código "Hello, World!":**
   Substitua o conteúdo do arquivo `src/main.rs` pelo seguinte código:
   ```rust
   fn main() {
       println!("Hello, World!");
   }
   ```

5. **Compile e execute o programa:**
   No terminal, dentro do diretório do seu projeto (`hello_world`), execute o seguinte comando para compilar e executar o seu programa Rust:
   ```bash
   cargo run
   ```
   Isso irá compilar seu programa e executá-lo. Você deve ver a saída "Hello, World!" impressa no terminal.

