# Prompts do RefeiçON

## Versão 1: o prompt usado na imersão (Gemini Canvas)

Escrito em dupla, depois de desligarmos o celular para pensar no problema e na solução. Está como foi enviado.

```text
Atue como um Arquiteto de Software Sênior, Desenvolvedor Front-End Expert e Especialista em UI/UX focado em produtos digitais para EdTech e aceleração de carreiras. Escreva e desenvolva no Gemini Canvas uma APLICAÇÃO, moderno e interativo em um único arquivo (HTML5, Tailwind CSS e JavaScript modular). A APLICAÇÃO não deve ser apenas uma caixa de chat de texto plano, mas sim uma interface interativa com painéis e botões clicáveis. O recurso deve resolver o seguinte problema: Recarregar bilhete do Restaurante Universitário tem mt fila e é apenas fisicamente. Ele deve ter fumcionakidade recarga pela interface. Na interface visual, apresente uma tela principal dinâmica que contenha este visual e nome: deve ser algo prático, a dona do cartão insere o código do cartão e senha do suap para confirmar os dados e add o valor da recarga e o tipo de pagamento, a interface pode mostrar a quantidade de refeições que a pessoa vai ter com aquele valor . Utilize uma linguagem jovem, direta e empática em toda a interface e nos feedbacks gerados pelo aplicativo. Forneça o código em um único arquivo HTML (autossuficiente e responsivo para desktop/mobile), com CSS e JS integrados. Inclua dados fictícios realistas para preencher o painel e assegure que a aplicação siga as regras INSTRUÇÕES DE ÉTICA E SEGURANÇA.
```

**O que funcionou:** papel bem definido, problema claro, pedido de interface com painéis e botões (não só chat), arquivo único e responsivo, tom de linguagem definido e dados fictícios.

**O que eu melhoraria:** citei "regras de ética e segurança" sem escrevê-las; faltaram regras de negócio (valor da refeição, valores mínimo e máximo), o fluxo passo a passo e critérios de acessibilidade. Também não deixei claro que é uma simulação.

## Versão 2: prompt melhorado (escrito depois, para a próxima iteração)

```text
Atue como Arquiteto de Software Sênior, Desenvolvedor Front-End e especialista em UX para EdTech.

PROBLEMA: recarregar o bilhete do Restaurante Universitário só é possível presencialmente, com muita fila.

PÚBLICO: estudantes de instituto federal, de 17 a 25 anos, que usam mais o celular.

ENTREGA: um único arquivo HTML (HTML5, Tailwind CSS via CDN e JavaScript), responsivo, com CSS e JS integrados. Interface com painéis e botões clicáveis, não um chat.

FLUXO (4 passos): 1) identificar o cartão; 2) escolher o valor da recarga; 3) escolher o pagamento (Pix, crédito ou boleto); 4) confirmar e mostrar o comprovante.

REGRAS DE NEGÓCIO (valores fictícios): refeição subsidiada a R$ 1,40; recarga mínima de R$ 7,00 e máxima de R$ [defina]. Mostrar em tempo real quantas refeições o valor compra e o saldo depois da recarga.

PAINEL: saldo, últimas recargas e refeições restantes, com dados fictícios realistas.

SEGURANÇA E ÉTICA: é uma simulação, com aviso visível na tela ("Protótipo, dados fictícios"). Nenhum dado real é enviado ou guardado. Campo de senha mascarado e nunca exibido. Não pedir dados além do necessário. Mensagens de erro que não revelem informação sensível.

ACESSIBILIDADE: bom contraste, navegação por teclado e textos de botão claros.

TOM: jovem, direto e empático em toda a interface e nos feedbacks.
```
