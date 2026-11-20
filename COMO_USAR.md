# como colocar no perfil (v4 animada)

1. No GitHub, crie (ou abra) o repositório **público** `joaozitoito`, com o mesmo nome do seu usuário.
2. Suba o `README.md` e a pasta `assets/` inteira na raiz. Se já tinha a versão antiga, substitua tudo e apague os SVGs velhos.
3. Em **Settings → General → Features**, deixe **Issues** ligado. O botão "recado" e o mural usam as issues como livro de visitas.

## o que se mexe

- **banner**: os olhos em ASCII atravessam da direita pra esquerda, cada um numa velocidade, e piscam de vez em quando. As dobras de fundo andam devagar, e o nome dá um corte de glitch a cada ~5 s.
- **faixa**: o rolo de filme corre; são os 8 quadros de um olho olhando em volta e piscando.
- **rodapé**: o olho vai fechando aos poucos, fica fechado e abre de novo.
- **tudo**: estática leve tremendo e scanlines por cima.

As animações são CSS dentro dos próprios SVGs, então rodam direto no navegador, sem script.
Se o GitHub mostrar a imagem antiga, recarregue com Ctrl+F5 (ele guarda cache das imagens).

## hierarquia

São só quatro níveis de texto, todos na mesma fonte (Anonymous Pro) e alinhados na mesma margem esquerda:

1. **nome**: grande, só no banner.
2. **títulos de seção**: 40 px em negrito, com o sigilo-olho e a linha `.:.:`.
3. **texto**: 21 px, mesmo tamanho em sobre, agora, projetos e mural.
4. **detalhes**: 14–18 px em cinza (usuário, frase do banner, botões, assinatura do rodapé).

Pra isso o texto das seções foi desenhado dentro das imagens, assim ele não troca de fonte no meio da página. O único texto solto do GitHub é o contador de visitas.

## o que editar

- **projetos e textos**: como agora fazem parte das imagens, é só me pedir a troca que eu gero o SVG de novo.
- **contador**: o número vem do komarev.com e conta as visitas de verdade.
- **fundo**: as imagens usam o mesmo preto do tema escuro do GitHub (#0d1117) e a estática some nas bordas, então os blocos emendam sem faixa entre eles. No tema claro aparecem como blocos escuros.
