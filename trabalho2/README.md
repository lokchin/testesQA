> Sistema da Pichau

# 1 - Requisitos Funcionais [RF]:

### RF1 - Funcionalidades Gerais:
- **Cenário de teste 1: Linguagens aceitas no campo de pesquisa**
  - CT 01: [Input de "i3 processor"], [Passou]
  - CT 02: [Input de "processador i3"], [Passou]
  - CT 03: [Input de "i3處理器"], [Exceção "500" lançada, não passou]

- **Cenário de teste 2: Campo de preenchimento de CEP**
  - CT 01: [Números entre [0,9]], [Limite de 8 números, com a adição automática de "-"]
  - CT 02: [Letras], [Não há input]
  - CT 03: [Caracteres especiais], [Não há input]

### RF2 - Montagem de computador:
- **Cenário de teste 1: Compatibilidade entre componentes**
  - CT 01: [Processador AMD com placa mãe Intel], [O sistema retira das buscas]
  - CT 02: [Processador AMD com placa mãe AMD], [Produto encontrado]
  - CT 03: [Processador Intel com placa mãe Intel], [Produto encontrado]
    
- **Cenário de teste 2: Quantidade de componentes compatíveis**
  - CT 01: [Quatro Memórias RAM caso a placa mãe aceite], [Passou]
  - CT 02: [Quatro Memórias HD/SSD caso a placa mãe aceite], [Passou]
  - CT 03: [Ventoínhas compatíveis com o gabinete], [Passou]

# 2 - Requisitos Não Funcionais [RNF]:

### RNF1 - Funcionalidades visuais:
- **Cenário de teste 1: Modo claro/escuro**
  - CT 01: [Alteração de tema na header], [Passou]
  - CT 02: [Alteração de tema na seção de produtos], [Passou]
  - CT 03: [Alteração de tema no footer], [Tema no modo escuro permanente, não passou]

- **Cenário de teste 2: Navegabilidade no sistema**
  - CT 01: [Seleção livre de componentes na montagem de computadores], [Não passou]
  - CT 02: [Seleção de departamentos], [Passou]
  - CT 03: [Acesso as telas do footer], [Passou]
    
### RNF2 - Acessibilidade:
- **Cenário de teste 1: Acesso por navegadores diferentes**
  - CT 01: [Acesso no Google Chrome], [Passou]
  - CT 02: [Acesso no Samsung Internet], [Passou]
  - CT 03: [Acesso no Internet Explorer (modo compatibilidade do MS Edge)], [Não passou]

- **Cenário de teste 2: O site precisa ser responsivo em dispositivos móveis**
  - CT 01: [iPhone SE], [Passou]
  - CT 02: [Samsung Galaxy S20 Ultra], [Passou]
  - CT 03: [iPad Air], [Passou]

# 3 - Integrante:

| Aluno                     | Professora                | Turma | Disciplina                     |
| ------------------------- | ------------------------- | ----- | ------------------------------ |
| Bruno Santos Lokchin | Gabriela Martins de Jesus | CC5N  | Qualidade e Testes de Software |
