# Plano de Teste

# E-commerce Pichau

### O que é a Pichau?
#### Sessão retirada de "Quem somos?"
> Fundada no ano de 2007, a Pichau Informática é uma empresa que trabalha com os mais variados produtos, atuando principalmente no setor de informática e equipamentos eletrônicos em geral, área bastante competitiva e em constante crescimento, onde qualidade, variedade, garantia e eficiência são critérios importantíssimos para total satisfação, confiança e preferência de nossos consumidores.
Além do nosso e-commerce possuímos uma loja física situada em Joinville/SC, onde temos a variedade de nosso site ao gosto dos mais exigentes clientes. Oferecemos não apenas a comodidade da compra online, mas também o tratamento olho no olho que muitos preferem e sempre confiam.
Procuramos acima de tudo oferecer o que há de melhor, os melhores fornecedores, os mais atualizados produtos, o mais atencioso dos atendimentos, juntamente com os preços mais competitivos e atraentes do mercado para que nosso público encontre não apenas variedade e qualidade, mas também uma empresa que se preocupa com a felicidade e total satisfação de seus clientes e por que não, amigos!



## 1 - Introdução

Este documento detalha o plano de testes abrangente para o ecommerce Pichau, com foco em garantir a qualidade, confiabilidade e funcionalidade da plataforma. Abrange a identificação de informações do projeto, componentes de software a serem testados, requisitos a serem validados, estratégias de teste, recursos necessários, estimativa de esforços e elementos resultantes.

Com esse documento, é possível:
- Identificar informações de projeto existentes e os componentes de software que devem ser testados.
- Listar os Requisitos a testar.
- Recomendar e descrever as estratégias de teste a serem empregadas.
- Identificar os recursos necessários e prover uma estimativa dos esforços de teste.
- Listar os elementos resultantes do projeto de testes.

## 2 - Requisitos

Esse documento de plano de testes aborda os requisitos funcionais fundamentais para o funcionamento do sistema.
São testados os requisitos:

Requisito | Descrição
-----------------------------|---------------------
IDREQ-1                       |       Seção de montagem de computadores
IDREQ-2                       |       Barra de pesquisa


## 3 - Tipos de teste

Esta seção deve conter os tipos de testes escolhidos para cada iteração do projeto.

### 3.1 Requisito 1: Seção de montagem de computadores

#### Teste de Interface
> O teste de interface de usuário (UI), também conhecido como teste de GUI (Graphical User Interface), foca em avaliar a usabilidade, funcionalidade, acessibilidade e estética da interface de um software, aplicativo ou site. Ele visa garantir que a interface seja intuitiva, fácil de usar, agradável esteticamente e atenda às expectativas dos usuários.

#### Por que esse teste?
> Por ser uma seção onde o usuário escolhe como montar um computador do zero, e que há muitas regras e condicionais para uma montagem correta, o que torma o usuário facilmente sucetível a erro, então optei pelo teste de usabilidade, um ramo do teste de interface.

#### O teste
> Ao iniciar a testagem, notei que as principais peças são escolhidas primeiro e em seguida o usuário pode escolher as peças compatíveis com a primeira escolhida. Por exemplo, caso escolha um processador da AMD, não aparecerá placas-mãe compatíveis apenas com Intel, ao escolher uma fonte, o sistema recomenda uma baseado no consumo das peças escolhidas. Os elementos de fato seguem a psicologia das cores e a navegabilidade facilitada.

### Parâmetros de teste
#### Clicabilidade
- Verifiquei se a interface realmente é clicável
#### Navegação
- O usuário consegue retornar e avançar facilmente nesse quesito
#### Psicologia das cores
- Veriquei se as cores dos elementos não infrigem a teoria da psicologia das cores, o que induziria o usuário ao erro caso não cumprido.

#### Conclusão
O Teste de Interface induz que um sistema falso com o intuito de aplicar golpes ao usuário infringe diversas áreas do teste de UX, pois induz o usuário ao erro. O que não acontece com o site da Pichau para montagem de computadores.

### Criticidade de Defeitos:
- Baixa: Checkbox com a marcação fora da caixa em alguns campos.
- Média: Configuração montada é perdida caso perca a conexão por breve momento.
- Alta: Falha na responsividade para acesso mobile.

<br/>
<table>
    <tr>
        <th>
            Objetivo
        </th>
        <th colspan="4">
            Verificar a usabilidade da seção de montagem de computadores
        </th>
    </tr>
    <tr>
        <th>
            Método de Execução
        </th>
        <th colspan="2">
            (x) manual
        </th>
        <th colspan="2">
            ( ) automática
        </th>
    </tr>
    <tr>
        <th>
            Nível de teste
        </th>
        <th>
            Integração ( )
        </th>
        <th>
            Sistema ( )
        </th>
        <th>
            Unidade (x)
        </th>
    </tr>
    <tr>
        <th>
            Técnica
        </th>
        <th colspan="2">
            Teste Estrutural ( )
        </th>
        <th colspan="2">
            Teste Funcional (x)
        </th>
    </tr>
    <tr>
        <th>
            Responsável(is)
        </th>
        <th colspan="4">
            Bruno Santos Lokchin
        </th>
    </tr>
</table>
<br/>

### 3.2 Requisito 2: Barra de Pesquisa

#### Teste exploratório
> O teste exploratório, também conhecido como teste ad-hoc, é uma abordagem dinâmica e flexível para testar software. Ao contrário dos testes tradicionais, que seguem um plano predefinido, o teste exploratório incentiva a exploração livre e criativa do software, permitindo a descoberta de falhas inesperadas e a identificação de áreas que podem ser aprimoradas.

#### Por que esse teste?
> A barra de pesquisa é aberta ao usuário, podendo pesquisar os produtos disponíveis na loja, uma teste de exploração é suficiente e eficaz para verificar a funcionalidade desse elemento.

#### O teste
> Realizando o teste, percebi que a Pichau possui uma dor de regra de negócio assim como muitos ecommerces, que é a falta de um Lógica de busca eficaz. Por exemplo, ao procurar por "Computador i3", aparecem os modelos específicos que possuem i3, ao procurar por "Processador i3", aparecem apenas os processadores, ao procurar apenas por "i3", o sistema mostra os computadores montados com i3 e não os processadores. Pesquisando algo fora de contexto, o sistema não retorna nenhum produto. Ao usar uma VPN e colocar para áreas remotas, há muitos produtos indisponíveis.

#### Conclusão
A barra de pesquisa funciona perfeitamente para o usuário que procura algo específico, mas dificulta para o usuário leigo.

### Parâmetros de teste
#### Lógica de busca
- A Lógica de busca é um fator importante em pesquisas, ajuda o usuário a encontrar o que procura, e no contexto técnico da Pichau, é fundamental.
#### Disponibilidade baseado em CEP
- Se algo pesquisado se encontra disponível ou não, baseado na localização do usuário.

### Criticidade de Defeitos:
- Baixa: Checkbox com a marcação fora da caixa em alguns campos.
- Média: Lógica de busca em conflito dependendo do que é pesquisado.
- Alta: Indisponibilidade dependendo do local.


<br/>
<table>
    <tr>
        <th>
            Objetivo
        </th>
        <th colspan="4">
            Verificar como a barra de pesquisa se comporta.
        </th>
    </tr>
    <tr>
        <th>
            Método de Execução
        </th>
        <th colspan="2">
            (x) manual
        </th>
        <th colspan="2">
            ( ) automática
        </th>
    </tr>
    <tr>
        <th>
            Nível de teste
        </th>
        <th>
            Integração ( )
        </th>
        <th>
            Sistema ( )
        </th>
        <th>
            Unidade (x)
        </th>
    </tr>
    <tr>
        <th>
            Técnica
        </th>
        <th colspan="2">
            Teste Estrutural ( )
        </th>
        <th colspan="2">
            Teste Funcional (x)
        </th>
    </tr>
    <tr>
        <th>
            Responsável(is)
        </th>
        <th colspan="4">
            Bruno Santos Lokchin
        </th>
    </tr>
</table>
<br/>

## 4 - Recursos

Esta seção deve descrever os recursos humanos, de ambiente de teste (hardware e software) e de ferramentas de automatização de testes necessários para execução dos testes que devem ser descritos nas subseções que seguem.

### 4.1 - Ambiente de teste - Hardware

Tipo de dispositivo| Processador          | Memória RAM
-------------------|----------------------|-------------
Notebook           | Intel Core i5 11300H | 16GB

### 4.2 - Ambiente de teste - Software

Sistema Operacinal | Navegador          | Versão do Navegador
-------------------|--------------------|-------------
Windows 11 Home    | Google Chrome      | 124.0.6367.156


### 4.2 SLA de Resolução
O SLA (Service Level Agreement) de resolução para cada nível de criticidade definida é fundamental para garantir que os problemas identificados sejam tratados de forma oportuna e eficiente. Abaixo estão os SLAs propostos para cada nível de criticidade:

- Baixa Criticidade: Resolução dentro de 5 dias úteis.
- Média Criticidade: Resolução dentro de 2 dias úteis.
- Alta Criticidade: Resolução dentro de 48 horas úteis.

#### Exemplos de SLAs de empresas:
1. DigitalOcean:
- Baixa Criticidade: Resolução dentro de 48 horas.
- Média Criticidade: Resolução dentro de 24 horas.
- Alta Criticidade: Resolução dentro de 4 horas.

2. Rackspace:
- Baixa Criticidade: Resolução dentro de 3 dias úteis.
- Média Criticidade: Resolução dentro de 1 dia útil.
- Alta Criticidade: Resolução dentro de 4 horas.
  
3. Heroku:
- Baixa Criticidade: Resolução dentro de 2 dias úteis.
- Média Criticidade: Resolução dentro de 1 dia útil.
- Alta Criticidade: Resolução dentro de 4 horas.

### 4.4 - Relatório de Defeito Identificado
#### Defeito 1:
**Descrição**: Ao abrir o site de montagens de computadores usando um dispositível móvel, alguns elementos e avisos terão uma sobreposição textual.

#### Criticidade
- Nível: Alto
- Impacto: Todos os usuários que acessam pelo celular, remove a credibilidade e profissionalismo do site.

#### Passos para reproduzir
1. Abra o navegador no celular.
2. Abra a seção de montagem de computadores.
3. Monte um computador de forma que forme um aviso, como "pouca memória RAM"

#### Resultados esperados
O site deve ser completamente responsivo.

#### Defeito 2:
**Descrição**: A Lógica de busca está sem acurácia, não busca produtos misturados nas primeiras alternativas

#### Criticidade
- Nível: Baixo
- Impacto: O sistema não facilita para usuários leigos em termos técnicos, o que acaba reduzindo vendas.

#### Passos para reproduzir
1. Abra o site no computador
2. Pesquise algo que possa gerar resultado ambíguo

### 5.0 - Intragrante

Aluno       |Professora        | Turma | Matéria
------------|------------------|-------|---------
Bruno Santos Lokchin | Gabriela Martins de Jesus | CC5N | Qualidade e Teste de Software
