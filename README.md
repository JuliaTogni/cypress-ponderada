# cypress-ponderada

## 1. O que é o Cypress e para que serve?

O Cypress é uma ferramenta de teste de front-end projetada para a web moderna. Ele foi desenvolvido para simplificar o processo de teste de aplicações web, permitindo que desenvolvedores e engenheiros de QA testem facilmente as funcionalidades de aplicações web de forma automatizada. O Cypress é utilizado para escrever testes de unidade, integração e ponta a ponta.

## 2. Vantagens e desvantagens do Cypress em relação a outras ferramentas de teste

### Vantagens:

- **Execução de testes em tempo real:** Cypress executa testes mais rapidamente ao rodar dentro do navegador
- **Facilidade de uso:** Sua sintaxe é fácil de entender e usar
- **Depuração simplificada:** Fornece snapshots e vídeos dos testes, facilitando a identificação de falhas de maneira visual
- **Testes End-to-End e de integração:** Suporta tanto testes de integração quanto end-to-end, sem a necessidade de configurações adicionais complexas

### Desvantagens:

- **Suporte limitado a navegadores:** Inicialmente limitado ao Chrome, mas agora suporta Firefox e Edge, com algumas limitações
- **Não é ideal para aplicativos móveis:** Focado em aplicações web, não sendo a melhor opção para testar aplicativos móveis nativos

## 3. Arquitetura do Cypress

A arquitetura do Cypress é única porque opera diretamente no mesmo loop de execução que a aplicação. Diferente de outras ferramentas que operam fora do navegador, o Cypress executa dentro do navegador, permitindo controle total sobre a aplicação, desde o carregamento de recursos até a execução de scripts assíncronos

## 4. Seletores de elementos no Cypress

Cypress usa seletores de elementos similares ao jQuery para identificar elementos HTML na página. Utiliza-se comandos como `cy.get()` e `cy.find()` para selecionar elementos baseados em classes, IDs, atributos, ou até combinações desses seletores

## 5. Comandos e asserções no Cypress

Os comandos no Cypress são utilizados para interagir com elementos na aplicação web (como clicar em um botão, digitar em um campo de texto, etc.), enquanto asserções são utilizadas para verificar se o estado da aplicação ou elemento está conforme o esperado. Exemplo: `cy.get('.my-element').should('exist').and('be.visible');`

## 6. Descrição das etapas de preparação de um teste de interface, execução e verificação no Cypress

1. **Preparação:** Comece configurando o ambiente de teste, incluindo a criação de dados de teste, como usuários, produtos ou informações relevantes, e a configuração do estado inicial da aplicação, como login, seleção de idioma, entre outros
2. **Execução:** Em seguida, escreva os scripts de teste que interagem com a aplicação, utilizando os comandos do Cypress para navegar pela aplicação, interagir com os elementos da interface, preencher formulários, clicar em botões e realizar as ações necessárias para cobrir os cenários de teste
3. **Verificação:** Por último, utilize as asserções para verificar se a aplicação está respondendo conforme o esperado após as interações, como a validação de mensagens de sucesso, verificação de conteúdo exibido na tela e confirmação do correto funcionamento de funcionalidades específicas

## 7. Como estruturar testes de forma eficiente no Cypress?

- **Organize os testes em suites:** Agrupe os testes relacionados em arquivos separados para manter o código de teste organizado de acordo com a funcionalidade ou componente testado.
- **Use `before()` e `beforeEach()` para preparação:** Essas funções ajudam a configurar o estado necessário antes de cada teste ou suite de testes, garantindo que as condições iniciais estejam sempre corretas.
- **Escreva testes claros e concisos:** Cada teste deve ser independente e focar em um aspecto específico da funcionalidade, evitando dependências desnecessárias entre os testes.
- **Aproveite os recursos do Cypress:** Utilize recursos como fixtures para dados de teste, comandos personalizados para ações específicas e plugins para estender as capacidades dos seus testes de forma eficiente.
