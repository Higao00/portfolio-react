
# Portfolio React

Este projeto é um **portfolio pessoal** desenvolvido utilizando **React**. Ele contém diversos recursos interativos e visuais, incluindo animações, formulários e integração com **EmailJS** para envio de mensagens diretamente do site.

## Tecnologias e Dependências

Este projeto utiliza as seguintes dependências para fornecer funcionalidades modernas e eficientes:

### Dependências

- **React** ![React](https://img.shields.io/badge/React-%2320232a.svg?style=flat&logo=react&logoColor=%2361DAFB)
  - Versão: `18.2.0`
- **React Router Dom** ![React Router](https://img.shields.io/badge/React%20Router-%23323330.svg?style=flat&logo=react-router&logoColor=%23CA4245)
  - Versão: `6.3.0`
- **Material UI** ![Material UI](https://img.shields.io/badge/Material%20UI-%23007FFF.svg?style=flat&logo=mui&logoColor=white)
  - `@mui/material`: Versão `5.10.3`
  - `@mui/icons-material`: Versão `5.10.3`
  - `@mui/lab`: Versão `5.0.0-alpha.101`
- **Framer Motion** ![Framer Motion](https://img.shields.io/badge/Framer%20Motion-%232D2F3F.svg?style=flat&logo=framer&logoColor=F7D9DC)
  - Versão: `7.2.1`
- **Styled Components** ![Styled Components](https://img.shields.io/badge/Styled%20Components-%23000000.svg?style=flat&logo=styled-components&logoColor=white)
  - Versão: `5.3.5`
- **Emotion** ![Emotion](https://img.shields.io/badge/Emotion-%23D76B72.svg?style=flat&logo=emotion&logoColor=white)
  - `@emotion/react`: Versão `11.10.4`
  - `@emotion/styled`: Versão `11.10.4`
- **EmailJS** ![EmailJS](https://img.shields.io/badge/EmailJS-%23F4D03F.svg?style=flat&logo=emailjs&logoColor=white)
  - Versão: `3.7.0`
- **React Hook Form** ![React Hook Form](https://img.shields.io/badge/React%20Hook%20Form-%23232F3E.svg?style=flat&logo=react-hook-form&logoColor=white)
  - Versão: `7.36.1`

### Dependências de Desenvolvimento

- **TypeScript** ![TypeScript](https://img.shields.io/badge/TypeScript-%23007ACC.svg?style=flat&logo=typescript&logoColor=white)
  - Versão: `4.6.4`
- **@babel/plugin-proposal-private-property-in-object** ![Babel](https://img.shields.io/badge/Babel-%23F9DC3E.svg?style=flat&logo=babel&logoColor=black)
  - Versão: `7.21.11`
- **@types**: Tipagens para várias dependências, incluindo React, Node e outros pacotes utilizados.
  - `@types/jest`, `@types/node`, `@types/react`, `@types/react-dom`, `@types/react-router-dom`, `@types/styled-components`.

### Scripts

Este projeto vem com alguns scripts básicos configurados para facilitar o desenvolvimento:

- **start**: Inicia o servidor de desenvolvimento.
  - `npm start`
- **build**: Cria a versão otimizada para produção.
  - `npm run build`
- **test**: Roda os testes configurados para o projeto.
  - `npm test`
- **eject**: Expõe as configurações internas do Create React App (se necessário).
  - `npm run eject`

### Browsers List

Este projeto é compatível com os seguintes navegadores:

- **Produção**: 
  - Mais de `0.2%` de participação de mercado global
  - Não obsoletos (não dead)
  - Não inclui o navegador `Opera Mini`

- **Desenvolvimento**:
  - Última versão do **Chrome**
  - Última versão do **Firefox**
  - Última versão do **Safari**
  
  
### Uso do Amazon S3
  O projeto faz uso do Amazon S3 para armazenar imagens e outros arquivos estáticos. O S3 é uma solução de armazenamento de objetos altamente escalável e durável, permitindo que você hospede e acesse esses arquivos de forma eficiente e segura.

  Configuração do Bucket S3:

  O bucket do S3 é configurado para armazenar imagens do site, garantindo que os recursos sejam carregados rapidamente e sem sobrecarregar o servidor.
  A configuração do bucket inclui permissões de leitura pública para que os usuários possam acessar os arquivos diretamente pela URL.
  Acesso aos Arquivos:

  As imagens são acessadas diretamente pelo seu endereço público gerado pelo S3, sem a necessidade de uma API intermediária.

## Como Rodar o Projeto

1. Clone este repositório para sua máquina local:

   ```bash
   git clone https://github.com/seu-usuario/portfolio-react.git
   ```

2. Instale as dependências do projeto:

   ```bash
   npm install
   ```

3. Execute o projeto localmente:

   ```bash
   npm start
   ```

   Isso abrirá o projeto no seu navegador padrão, geralmente acessível em `http://localhost:3000`.

## Como Enviar E-mails

Este projeto integra **EmailJS** para enviar e-mails diretamente do seu formulário de contato. Para que o envio de e-mails funcione corretamente, é necessário configurar a integração com o **EmailJS**.

1. Crie uma conta em [EmailJS](https://www.emailjs.com/).
2. Crie um novo **serviço de e-mail** e **modelo de e-mail**.
3. Adicione as variáveis de ambiente no seu arquivo `.env`:

   ```
   REACT_APP_YOUR_SERVICE_ID=seu-service-id-aqui
   REACT_APP_YOUR_TEMPLATE_ID=seu-template-id-aqui
   REACT_APP_YOUR_PUBLIC_KEY=seu-public-key-aqui
   ```

4. O envio de e-mail será feito automaticamente ao submeter o formulário.

## Contribuição

Sinta-se à vontade para fazer contribuições! Se você tiver sugestões ou melhorias, envie um **pull request** ou abra um **issue**.

