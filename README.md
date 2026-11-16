# Xeque-Mago

Estratégia de turnos em voxel: cada jogador tem um **Mago**, que é o rei, e um exército de bonecos.
Derrube o Mago inimigo para vencer, sem perder o seu.

![Mapa-Mundi](imagens/16_mapa_mundi.jpg)

## Baixar e jogar (Windows)

1. Abra a aba **[Releases](../../releases/latest)** e baixe `XequeMago-v0.6-windows.zip`.
2. Extraia o zip numa pasta.
3. Rode `XequeMago.exe`. Os dois arquivos (`.exe` e `.pck`) precisam ficar na mesma pasta.

Se o Windows mostrar "O Windows protegeu o computador", clique em **Mais informações → Executar assim mesmo**
(o jogo ainda não é assinado digitalmente).

Requisitos: Windows 10 ou 11 (64 bits) e placa de vídeo com Vulkan.
Se o jogo pesar no seu PC, vá em **Opções → Qualidade gráfica** e escolha **Baixa** ou **Média**.

![Menu](imagens/01_menu.png)

## Modos

- **Mapa-Mundi**: escolha um lugar da Grande Floresta e batalhe ali, **contra a CPU** ou com **dois jogadores**
  no mesmo computador, no estilo **Normal** ou **Turno-Mútuo**
- **Tutorial**: 11 lições curtas, uma para cada parte do jogo
- **Treino**: um campo com bonecos de pancada para testar os golpes de qualquer boneco

## Mapa-Mundi

O mundo é uma maquete em miniatura. Por enquanto só a **Grande Floresta** está pintada; o resto do continente
ainda é gesso com o desenho a lápis e vai ganhando cor a cada versão. Arraste para andar, gire com o botão
direito e aproxime com a roda. Clicando num lugar, abre o painel com a prévia da arena de luta.

Cada lugar é um local de verdade, com casas, gente andando e coisas para ver:

| Lugar | O que tem |
|---|---|
| Vila dos Lenhadores | Cabanas de tronco, pátio com pilhas de toras, fogueira e lenhadores rachando lenha |
| Vila Élfica | Casas de telhado pontudo e casas nas árvores, lampiões verdes e o campo de treino das arqueiras |
| Ruínas do Golem | Um vale atrás da montanha, só alcançado pelo túnel do rio; uma ruína meio aberta sob uma laje de rocha enorme, onde dorme o primeiro Golem |
| Lar da Árvore Anciã | A árvore mais velha do mundo, com raízes enormes, vagalumes e o lago |
| Floresta das Fadas | Sempre primavera: árvores rosadas e círculos de cogumelos que brilham |
| Estalagem da Encruzilhada | Onde todas as trilhas se cruzam: estalagem, estrebaria, carroças e viajantes |

![Vila dos Lenhadores](imagens/17_vila_dos_lenhadores.jpg)

![Vila Élfica](imagens/18_vila_elfica.jpg)

![Ruínas do Golem, atrás da montanha](imagens/19_ruinas_do_golem.jpg)

![O túnel do rio](imagens/21_tunel_do_rio.jpg)

![Estalagem da Encruzilhada](imagens/20_estalagem.jpg)

![Lar da Árvore Anciã](imagens/22_arvore_ancia.jpg)

No meio da mata ainda há lugares soltos em clareiras (Totem Gigante, Torre do Vigia, Torre Partida, Círculo de
Menires, Poço dos Desejos, Estátua Esquecida, cabanas e um acampamento) que vão ganhar uso nas próximas versões.

![Lugares da mata](imagens/23_lugares_da_mata.jpg)

### Arenas de luta

Como num jogo de monstrinhos, o lugar onde se anda e o lugar onde se luta são diferentes: a arena é uma "média" do
lugar, sem casas nem gente. Na dos lenhadores há tocos e uma tora atravessada no meio da pista; na ruína, lajes,
colunas partidas e um muro caído; na Árvore Anciã, raízes enormes; nas fadas, cogumelos gigantes; na
encruzilhada, a estrada de terra cruzando o campo e caixotes caídos de uma carroça.

![As seis arenas](imagens/25_arenas.jpg)

![Painel do lugar](imagens/24_painel_turno_mutuo.jpg)

## Turno-Mútuo

Além do estilo **Normal** (um jogador de cada vez), dá para jogar no **Turno-Mútuo**: os dois planejam escondido e
tudo acontece ao mesmo tempo, o que deixa a partida bem difícil de prever. Escolha o estilo no painel do lugar.

1. Os dois jogadores planejam sem ver o plano do outro (contra outra pessoa, o jogo pede para passar a vez).
2. Poderes do Mago, trocas de peça e posturas de defesa saem primeiro; depois os troncos e pedras quebrados.
3. Todos andam juntos. Dois bonecos indo para a mesma casa rolam o D20: o maior entra, e no empate ninguém entra.
   Dois que trocariam de lugar trombam e ficam onde estavam.
4. Um golpe numa casa de onde o alvo saiu se perde.
5. **Choque**: dois bonecos que se atacam na mesma rodada rolam o D20. O maior golpeia e o golpe do outro se perde;
   no empate, os dois golpeiam.
6. Os outros golpes saem numa ordem sorteada.

![Planejando no Turno-Mútuo](imagens/26_turno_mutuo.jpg)

## Tutorial

Cada lição monta um cenário próprio e guia clique a clique: o painel explica a mecânica, mostra o
próximo clique e marca a casa certa. As lições feitas ficam marcadas.

![Lições](imagens/11_licoes.png)

1. Andar e câmera · 2. Atacar e energia · 3. O dado de 20 lados · 4. Tipos de golpe e a ficha · 5. Terreno ·
6. Santuário · 7. Quebrar os totens · 8. O escudo do Mago · 9. Seu Mago · 10. Eventos do mapa · 11. Derrubar o Mago

![Lição do escudo](imagens/09_tutorial.png)

## Campo de Treino

Escolha qualquer boneco e bata nos bonecos de pancada: um colado, dois a 3 casas, um a 5 e um a 7 casas, mais um
aliado de pancada para os golpes de aliado. Eles voltam com a vida cheia a cada turno, e a energia infinita pode
ser ligada ou desligada. No canto de cima, a ficha do boneco em uso mostra a vida e a energia; passando o mouse num
golpe, as bolinhas de energia que ele gasta ficam vermelhas.

![Treino](imagens/12_treino.png)

## Como funciona

![Escudo do Mago](imagens/03_guarda_do_mago.png)

A defesa do Mago tem **três etapas**:

1. **Os dois totens de pé.** Cada lado tem dois totens nos flancos. Enquanto os dois estão de pé, nada atinge o
   Mago, nem o escudo dele, e ele só usa magias de suporte (cura, escudo, potencializar, mudar o terreno),
   que alcançam a arena inteira.
2. **Um totem caído.** Os golpes no Mago passam a quebrar o escudo de energia que o cerca (12 de vida), e o Mago
   libera o seu ataque principal.
3. **Escudo quebrado.** O Mago usa todos os ataques, as magias caem para 4 casas de alcance e ele passa a levar dano.

![Totem](imagens/07_totem.png)

- **Exército.** Cada lado monta o exército com **30 pontos** numa área de 10x4 casas e começa com **5 de mana**
  (sobe 1 por rodada, até 10).
- **Quebrar.** Todo boneco (menos o Mago) pode quebrar de uma vez um tronco, pedra ou muro colado nele. Gasta o
  ataque do turno, mas ele ainda pode andar depois e passar pela brecha.
- **Santuários.** O boneco que chega a um santuário dourado escolhe uma bênção que vale até o fim da partida:
  **Ataque** (+2 de dano), **Defesa** (defende com 3 a menos no dado) ou **Velocidade** (+1 casa por movimento).
  Cada boneco recebe uma bênção por partida.
- **Dado de 20 lados.** Todo ataque com dano rola um d20 contra um mínimo calculado pelos atributos; o alvo rola a
  defesa. 1 sempre erra; 20 é crítico (+50% de dano, sem defesa).
- **Energia.** Cada golpe gasta energia do boneco. Golpes básicos custam 2 ou 3; os grandes, de 6 a 8. A energia volta
  devagar e cada boneco tem o seu ritmo:

  | Recupera por turno | Bonecos |
  |---|---|
  | 2 | Lobo Sombrio, Fantasma, Árvore Anciã, Geomante, Maga das Marés |
  | 1 | Minotauro, Golem, Yeti, Titã de Lava, Arqueira Élfica, Goblin Catapulta, Verme das Dunas |
  | 1, ou 2 ao lado de fogo | Salamandra |

![Duelo de dados](imagens/04_duelo_de_dados.png)

## Tipos de golpe

Todo golpe tem um tipo, com ícone e cor no menu e na ficha:

| Tipo | O que faz |
|---|---|
| Golpe Base | Ataque ou movimento principal |
| Proteção Pessoal | Protege ou recupera o próprio boneco |
| Proteção de Aliado | Ajuda um boneco do seu time |
| Mudança de Área | Muda o chão ou o ar de uma região (espinhos, lava, chão escaldante, areia, pólen, gelo) |
| Mudança de Status | Fortalece o boneco ou enfraquece o inimigo |
| Muralha | Ergue paredes altas que sobem do chão |

![Golpes com tipo](imagens/05_classes_e_golpes.png)

Alguns golpes: Flechada Potente (a exatamente 7 casas), Recuo Forçado, Meditação Élfica, Bomba de Espinhos,
Muro de Tronco, Pólen Atordoante, Drenagem, Mergulho, Tempestade de Areia, Abalo Sísmico, Arremesso de Rocha,
Salto Ígneo, Bola de Neve que cresce, Muro de Gelo, Mãos Penumbrais, Último Desejo, Território Vulcânico e
Muro de Obsidiana.

![Muro de troncos](imagens/13_muro_de_troncos.png)

![Pólen](imagens/14_polen.png)

![Lava e obsidiana](imagens/15_lava_e_obsidiana.png)

## Classes

| Classe | Bonecos | Papel |
|---|---|---|
| Tanque | Golem, Minotauro, Yeti, Titã de Lava | Aguenta golpes, segura a linha, protege |
| Assassino | Lobo Sombrio, Salamandra, Verme das Dunas | Entra pelos flancos e finaliza |
| Atirador | Arqueira Élfica, Goblin Catapulta (gigante 2x2) | Age de longe e muda o terreno |
| Suporte | Árvore Anciã, Fantasma, Geomante, Maga das Marés | Cura, protege e controla |

Na escolha do exército, o botão **!** ao lado de cada boneco abre a ficha dele: classe, passiva, atributos e golpes.

![Ficha do boneco](imagens/10_ficha.png)

## Eventos aleatórios

Cada arena tem 3 eventos. Cada evento é anunciado uma rodada antes num cartaz no meio da tela, com as casas
atingidas marcadas em vermelho; quando acontece, aparece o efeito no tabuleiro (chuva, neve, areia, pedras caindo...)
e, se durar mais de uma rodada, um aviso no canto mostra quantas rodadas faltam:

| Arenas | Eventos |
|---|---|
| Grande Floresta (Lenhadores, Élfica, Árvore Anciã, Fadas, Encruzilhada) | Névoa Fina, Raízes Vivas, Chuva de Verão |
| Ruínas do Golem | Desabamento, Cristal Ressonante, Escuridão |

Os mapas do deserto, do pântano e da neve voltam quando essas regiões forem pintadas no Mapa-Mundi.

![Evento: névoa](imagens/06_evento_nevoa.png)

![Lago](imagens/08_lago.png)

## Controles

- **W A S D**: mover a câmera
- **Botão esquerdo + arrastar**: girar
- **Roda do mouse**: aproximar
- **Botão direito**: voltar um passo
- **Esc**: menu

## Feedback

Jogou? Conte o que achou na aba **[Issues](../../issues)**: o que ficou confuso, o que está forte ou fraco demais,
bugs e ideias. Prints ajudam muito.

---

Versão 0.6 (protótipo). Feito com Godot 4.5. Este repositório traz apenas o jogo para download;
o código-fonte não está público.
