# RefeiçON: recarga do bilhete do RU sem fila

> **Protótipo com dados fictícios.** Nenhum dado real é enviado, guardado ou processado. Feito em uma imersão do Gemini Lab, com vibe coding no Gemini Canvas.

[**Ver demo online**](https://giovanna-dantas.github.io/refeicon-recarga-ru/) · [Ver o prompt](PROMPT.md)

![Tela principal do RefeiçON](img/tela-principal.png)

## O problema

Recarregar o bilhete do Restaurante Universitário (RU) só dá para fazer presencialmente. Isso gera fila, e quem tem aula logo depois perde tempo ou até a refeição.

## A solução

Um protótipo de interface em que a pessoa recarrega o bilhete em 4 passos, pelo celular ou pelo computador:

1. Identifica o cartão (matrícula do estudante)
2. Escolhe o valor da recarga (R$ 7, R$ 14, R$ 28, R$ 50 ou valor livre)
3. Escolhe a forma de pagamento (Pix, crédito ou boleto)
4. Vê quantas refeições aquele valor compra e confirma

Também tem painel com saldo, histórico e extrato, e horário de funcionamento do RU.

| Recurso | O que faz |
|---|---|
| Calculadora de refeições | Mostra na hora quantas refeições o valor da recarga garante (ex.: R$ 7,00 = 5 refeições, com refeição subsidiada a R$ 1,40) |
| Atalhos de valor | Botões prontos para as recargas mais comuns |
| Histórico e extrato | Lista de recargas e consumo (dados fictícios) |
| Linguagem da interface | Jovem, direta e empática, definida no prompt |

## Como eu usei IA (e o que foi decisão minha)

**Ferramenta:** Gemini Canvas (vibe coding). O código foi gerado pela IA a partir de um prompt que eu escrevi em dupla com a [@NOME-DA-MARI](https://github.com/).

**Método:** antes de abrir o Gemini, desligamos o celular e pensamos por conta própria no problema e na solução. Só depois escrevemos tudo em um único prompt.

| Decisão minha | Decisão da IA |
|---|---|
| Qual problema resolver e para quem | Estrutura do código (HTML, Tailwind e JavaScript) |
| O fluxo da recarga e as telas | Layout visual e componentes |
| Regras de negócio (valor da refeição, valores de recarga) | Textos de apoio dentro da interface |
| Tom da linguagem | Dados fictícios de exemplo |
| Regras de ética e segurança | |

O prompt completo, junto com uma versão melhorada que escrevi depois, está em [PROMPT.md](PROMPT.md).

## O que eu aprendi

- **Prompt bom nasce do pensamento, não da ferramenta.** Quanto mais claro o problema, o público e as regras, melhor o resultado.
- **A IA acelera, mas a decisão é humana.** Escolher o problema, o fluxo e os limites de segurança foi trabalho nosso.
- **Segurança precisa entrar no desenho.** Revisando o protótipo, vi que pedir senha em uma tela própria não seria aceitável num produto real (veja abaixo).
- **Prompt incompleto vira lacuna.** O primeiro prompt citava "instruções de ética e segurança" sem escrevê-las. Na versão melhorada, eu defini essas regras.

## Ética e segurança

- É uma **simulação**, com aviso visível na tela.
- Todos os dados (matrícula, saldo, histórico) são **fictícios**.
- Nada é enviado para servidor nem salvo.
- O campo de senha é só ilustrativo e **nunca deve receber a senha real de ninguém**.
- Em uma versão real, o acesso teria que usar **login oficial da instituição**, com autorização, sem o aluno digitar a senha do SUAP em tela de terceiros.

## Limitações

- Não há back-end: a recarga é simulada.
- Não há pagamento real nem integração com o SUAP.
- Não foi testado com estudantes de verdade.

## Próximos passos

- [ ] Conversar com 5 a 10 estudantes do RU e medir o tempo médio de fila hoje
- [ ] Trocar o login simulado por autenticação oficial da instituição
- [ ] Integrar pagamento Pix por uma API real
- [ ] Adicionar um assistente de IA para tirar dúvidas ("quantas refeições me restam esta semana?")
- [ ] Testar acessibilidade (contraste e navegação por teclado)

## Como rodar

Não precisa instalar nada. Baixe o arquivo `index.html` e abra no navegador, ou acesse a demo online acima.

## Habilidades que este projeto mostra

- Prompt engineering aplicado a um problema real
- Vibe coding com Gemini Canvas
- Product thinking: problema, público, fluxo e regras
- Preocupação com ética e privacidade desde o desenho
- Trabalho em dupla e documentação

## Autoria

Criado por **Giovanna Dantas** e **[@NOME-DA-MARI]** durante o Gemini Lab, no IFSP.

[LinkedIn](https://www.linkedin.com/in/giovanna-dantass/)
