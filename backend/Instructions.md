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

# Exercício A: Quake log Parser

Consumo dos dados: [Games Logs](https://github.com/rubcube/hiring-exercises/blob/master/backend/games.log)

## História 1

Eu como administrador do jogo, quero poder analisar a quantidade de mortes por causa, a quantidade de mortes pelo `<world>` e ranking geral de kills por jogador, para acompanhamento de indicadores que possam causar anomalias dentro do jogo, como balanceamento de armas, hackers, etc.

Exemplo:

```json
"game-1": {
	kills_by_means: {
		"MOD_SHOTGUN": 10,
		"MOD_RAILGUN": 2,
		"MOD_GAUNTLET": 1,
		"XXXX": N
	},
	general_ranking: {
		"Dono da bola": 15,
    "Isgalamido": 10,
    "Zeh": 5
	},
	killed_by_world: {
		"Dono da bola": 5,
    "Isgalamido": 2,
    "Zeh": 0
	}
}
```

## História 2

Eu como administrador do jogo, quero poder consumir esses dados da História 1, de forma estruturada por meio de uma API,  para montar uma visualização desses dados por jogo, levando em consideração os seguintes tipos de causas de morte (retirado do [código-fonte](https://github.com/id-Software/Quake-III-Arena/blob/master/code/game/bg_public.h)):

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

# Enviando o teste

Veja as instruções de envio [aqui](https://github.com/rubcube/hiring-exercises/blob/master/README.md)