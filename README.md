🏁 Mini Jogo de Corrida com Confrontos (NODE.JS)

Este projeto simula uma corrida divertida entre dois personagens: **Mario** e **Luigi**, usando lógica baseada em sorte (rolagem de dados) e atributos personalizados.

🎮 Regras do Jogo

- A corrida acontece em **5 rodadas**.
- A cada rodada, é sorteado um tipo de **bloco**:
  - `RETA`: usa o atributo `VELOCIDADE`.
  - `CURVA`: usa o atributo `MANOBRABILIDADE`.
  - `CONFRONTO`: usa o atributo `PODER`, e o personagem perdedor perde 1 ponto (se tiver).
- O personagem que obtiver o maior total na rodada marca **1 ponto**.
- Ao final das 5 rodadas, quem tiver mais pontos vence!

🧠 Como funciona

- Atributos dos personagens:
  const player1 = {
    NOME: "Mario",
    VELOCIDADE: 4,
    MANOBRABILIDADE: 3,
    PODER: 3,
    PONTOS: 0,
  };

  const player2 = {
    NOME: "Luigi",
    VELOCIDADE: 3,
    MANOBRABILIDADE: 4,
    PODER: 4,
    PONTOS: 0,
  };

A cada rodada:

É sorteado o tipo de bloco (reta, curva ou confronto).

Cada personagem rola um dado (de 1 a 6).

O valor do dado é somado ao atributo correspondente.

O personagem com maior resultado ganha a rodada.
