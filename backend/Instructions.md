# Exercício Backend

```
TEMPO:        48 horas máximo após recebimento da notificação via email.
LINGUAGENS:   TypeScript/Javascript/.NET
FRAMEWORKS:   NestJS/ExpressJS/Fastify/.NET Framework e quaisquers bibliotecas que achar necessário
TESTES:       legal ter, mas não é obrigatório
DOCUMENTAÇÃO: legal ter, mas não é obrigatório
```

# Instruções Gerais

Este exercício consiste em implementar a melhor solução possível para um dos exercícios abaixo no tempo previsto. Estamos avaliando sua capacidade de atender a um conjunto de requisitos e criar uma solução completa que demonstre habilidade, consideração e arquitetura. Este NÃO é um teste de quão bem você conhece Typescript/NestJS/Fastify/.NET, nem deve tentar nos impressionar com soluções muito complexas. Se você quer nos impressionar, construa algo bonito, intuitivo e fácil de depurar/testar/estender 🫡.

Idealmente, sua solução teria alguma maneira de ser executada localmente e visualizar os resultados em um emulador para que possamos analisar totalmente a experiência e não apenas o código-fonte.

# Exercício: Quake log Parser

Consumo dos dados: [Games Logs](https://github.com/rubcube/hiring-exercises/blob/master/backend/games.log)

Tipos de morte [(código-fonte)](https://github.com/id-Software/Quake-III-Arena/blob/master/code/game/bg_public.h):

```c
// means of death
typedef enum {
	MOD_UNKNOWN,
	MOD_SHOTGUN,
	MOD_GAUNTLET,
	MOD_MACHINEGUN,
	MOD_GRENADE,
	MOD_GRENADE_SPLASH,
	MOD_ROCKET,
	MOD_ROCKET_SPLASH,
	MOD_PLASMA,
	MOD_PLASMA_SPLASH,
	MOD_RAILGUN,
	MOD_LIGHTNING,
	MOD_BFG,
	MOD_BFG_SPLASH,
	MOD_WATER,
	MOD_SLIME,
	MOD_LAVA,
	MOD_CRUSH,
	MOD_TELEFRAG,
	MOD_FALLING,
	MOD_SUICIDE,
	MOD_TARGET_LASER,
	MOD_TRIGGER_HURT,
#ifdef MISSIONPACK
	MOD_NAIL,
	MOD_CHAINGUN,
	MOD_PROXIMITY_MINE,
	MOD_KAMIKAZE,
	MOD_JUICED,
#endif
	MOD_GRAPPLE
} meansOfDeath_t;
```

## História 1

Eu como administrador do jogo, quero ter a estatística por jogo, do total de mortes, de mortes por causa e de mortes causadas pelo `<world>` para entender dificuldade dos jogadores.

## História 2

Eu como player, quero ver o ranking de cada partida para saber o vencedor e meu desempenho. 

**Critérios de aceite:**

- Os jogadores começam com zero pontos
- A cada kill o jogador ganha um ponto
- A cada morte pelo mundo o jogador perde um ponto
- É permitido pontuação negativa
- O `<world>` não deve entrar no ranking de jogadores
- Os jogadores podem mudar de nome no meio da partida, mas só o último nome deve ser considerado no ranking

## História 3

Eu como administrador do jogo, quero poder consultar as estatísticas de um jogo específicou ou de todos os jogos de maneira estruturada por uma API para montar uma visualização para os jogadores

# Enviando o teste

Veja as instruções de envio [aqui](https://github.com/rubcube/hiring-exercises/blob/master/README.md)
