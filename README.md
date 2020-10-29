# Ranking dos gastos dos Deputados

Estamos muito felizes que você tenha chegado nessa etapa do nosso processo seletivo, para essa fase, desejamos que você resolva um desafio. Nosso desafio consiste em analisar alguns dados disponibilizados pelo Câmara dos Deputados relativos aos gastos dos parlamentares. A ideia é descobrir quem, do seu estado, está gastando mais e exibir de forma resumida esses principais gastos.

## Objetivo do Projeto

Você já ouviu falar da CEAP? A Cota para o Exercício da Atividade Parlamentar, custeia as despesas do mandato, como passagens aéreas e conta de celular. Algumas são reembolsadas, como as com os Correios, e outras são pagas por débito automático, como a compra de passagens. Nos casos de reembolso, os deputados têm três meses para apresentar os recibos. O valor mensal não utilizado fica acumulado ao longo do ano. Por esse motivo, em alguns meses o valor gasto pode ser maior que a média mensal. (Fonte: [Portal da Câmara dos Deputados](https://www2.camara.leg.br/transparencia/acesso-a-informacao/copy_of_perguntas-frequentes/cota-para-o-exercicio-da-atividade-parlamentar))


Através do portal da transparência, nós temos acesso a essas despesas e podemos saber como e onde os políticos estão gastando. **O objetivo é fazer uma aplicação que irá ler um arquivo CSV com os gasto de 2020 e oferecer as seguintes funcionalidades:**

- Listagem dos deputados do seu estado;
- Mostrar o somatório dos seus gastos;
- Listar as despesas, mostrando a data(`datEmissao`), estabelecimento(`txtFornecedor`), valor(`vlrLiquido`), e link para a nota(`urlDocumento`)
- Destacar a maior despesa do candidato

## Base de dados e explicações complementares

- [Explicação dos campos do arquivo CSV](https://www2.camara.leg.br/transparencia/cota-para-exercicio-da-atividade-parlamentar/explicacoes-sobre-o-formato-dos-arquivos-xml)
- [Fonte de dados (pegar o referente ao ano 2020 em formato CSV)](https://dadosabertos.camara.leg.br/swagger/api.html#staticfile)
- Ignorar linhas que não tenham no campo `sgUF` o estado que você mora. O objetivo do trabalho é focar apenas no seu estado;
- Considerar para fins de cálculos de despesa, o campo `vlrLiquido`. Esse é o valor que de fato foi debitado da cota do candidato;
- Dica para pegar a foto do político: **http://www.camara.leg.br/internet/deputado/bandep/{ideCadastro}.jpg**

# Requisitos
- Ter uma cobertura de código;
- Organizar estrutura do projeto utilizando padrões de projetos;

# Requisitos bônus
Esses requisitos não são obrigatórios, mas serão levados em consideração como pontos extras no momento da avaliação.

- A aplicação ser hospedada no Heroku, AWS ou similares;
- Evitar N + 1 nas queries;

# Critérios de avaliação

- Organização do projeto: Avalia a estrutura do projeto, documentação e uso de controle de versão;
- Coerência: Avalia se os requisitos foram atendidos;
- Boas práticas: Avalia se o projeto segue boas práticas de desenvolvimento, incluindo segurança e otimização;

O desafio deve ser entregue nos passando a URL de seu repositório. Fique a vontade caso queira incrementar o projeto com outras feautures não listadas aqui. Será visto como um extra.

Qualquer dúvida em relação ao desafio, responderemos por e-mail.

Bom trabalho!

