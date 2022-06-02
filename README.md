# JORNADA_DO_HEROI
const prompt = require("prompt-sync")(); 
console.clear()

let pontuacao = 0
let espada = 0 
let armadura = 0
let capacete = 0
let ninja_sagrado= 0
let po_magico = 0
let governo

console.log("A JORNADA DO HERÓI ")

let jogador = prompt("Digite o nome do(a) jogador(a) para começar: ")
while (jogador.length < 4) {
    console.log("\nDigite um nome de, pelo menos, 4 letras.")
    jogador = prompt("Digite o nome do(a) jogador(a) para começar: ")
}

console.log("\nOPÇÕES DE PERSONAGENS: \n[1] Liu Kang, um monge extremamente habilidoso na arte do combate. \n[2] Sub-zero Com uma incrível habilidade de controlar o gelo de diferentes maneiras,Sub-Zero demonstra toda sua autoconfiança para derrotar os oponentes .\n")
let personagem = +prompt("Escolha um personagem. Número [1] ou [2]: ")
while (personagem != 1 && personagem != 2) {
    console.log("\nNÚMERO INVÁLIDO!")
    personagem = +prompt("Escolha um personagem. Número [1] ou [2]: ")
}
console.clear()

let introducao1 = prompt("\n Apos a queda de um meteoro a terra foi invadida por lagartos gigantes...")
if (personagem == 1) {
    let introducao2 = prompt("\nVocê,grande guerreiro, precisa partir de imediato para  combater essa grande praga.")
} else {
    let introducao2 = prompt("\Você,grande guerreiro, precisa partir de imediato para  combater essa grande praga.")
}

let introducao3 = prompt("\n Grande guerreiro precisara se preparar para esse combate.")
let introducao4 = prompt(`\Voce esta preparado para essa aventura?`)

if (personagem == 1) {
    let i = prompt(`\n'${jogador},Vamos nessa!'`)
} else {
    let i = prompt(`\n'${jogador}, Estamos contando com voce.'`)
}

let a = +prompt("Você ira levar a sua espada? 1.[SIM] 2.[NÃO]")
while (a != 1 && a != 2) {
    console.log("\nNÚMERO INVÁLIDO!")
    a = +prompt("Você ira levar a sua espada 1.[SIM] 2.[NÃO]")
}
if (a == 1) {
    console.log("\n a espada esta em suas maos.")
    espada++
    pontuacao++
} else if ( a== 2) {
    console.log("\nVocê diz: \n'Nao preciso de espada, tenho os meus punhos!' \n.")
}
let b = +prompt("Vai levar sua armadura? 1.[SIM] 2.[NÃO]")
while (b != 1 && b != 2) {
    console.log("\nNÚMERO INVÁLIDO!")
    b = +prompt("Vai levar sua armadura? 1.[SIM] 2.[NÃO]")
}
if (b == 1) {
    let j = prompt("\n Voce esta protegido com a sua armadura.")
    pontuacao++
    armadura++
} else if ( b== 2) {
    let j = prompt("\nVocê confia em suas habilidades de desvio, nao precisara de armadura.")
}

let c = +prompt("Vai levar o seu capacete ? 1.[SIM] 2.[NÃO]")
while (c != 1 && c != 2) {
    console.log("\nNÚMERO INVÁLIDO!")
    c = +prompt("Vai levar o seu capacete? 1.[SIM] 2.[NÃO]")
}
if (c == 1) {
    let k = prompt("\nVocê esta mais protegido com o seu capacete.")
    pontuacao++
    capacete++
} else if ( c == 2) {
    let k = prompt("\n Voce parte sem o capacete.")
}
let d = +prompt("Você ira chamar o ninja_sagrado? 1.[SIM] 2.[NÃO]")
while (d != 1 && d != 2) {
    console.log("\nNÚMERO INVÁLIDO!")
    d = +prompt("Você ira chamar o ninja_sagrado 1.[SIM] 2.[NÃO]")
}
if (d == 1) {
    let l = prompt("\n o ninja_sagrado parte junto com voce.")
    pontuacao++
    ninja_sagrado++
} else if ( d == 2) {
    let l = prompt("\nVocê nao chama o ninja sagrado e parte sozinho")
}

if (personagem == 1) {
    
    let e = +prompt("Voce ira usar o po_magico? 1.[SIM] 2.[NÃO]")
    while (e != 1 && e != 2) {
     console.log("\nNÚMERO INVÁLIDO!")
     e = +prompt("Voce ira usar o po_magico? 1.[SIM] 2.[NÃO]")
}
if (e == 1) {
    let m = prompt("\nVocê acaba de ganhar novas habilidades.")
    pontuacao++
    po_magico++
} else if ( e == 2) {
    let m = prompt("\nVoce esta partindo sem o po magico.")
}
} else {
    let e = +prompt("Voce precisara do apoio do governo? 1.[SIM] 2.[NÃO]")
    while (e != 1 && e != 2) {
     console.log("\nNÚMERO INVÁLIDO!")
     e = +prompt("Voce precisara do apoio do governo? 1.[SIM] 2.[NÃO]")
}
if (e == 1) {
    let m = prompt("\Voce decide contatar o governo.")
    pontuacao++
    governo++
} else if ( e == 2) {
    let m = prompt("\nVoce acredita que nao ira precisar do apoio do governo.")
}
}

if (espada == 1) {
    let espada = prompt("\nA ESPADA FOI DE GRANDE AJUDA")
} else {
    let espada = prompt("\A ESPADA FOI DE GRANDE AJUDA")
}

if (armadura == 1) {
    let armadura = prompt("\nA ARMADURA IMPEEDIU GRANDES FERIMENTOS")
} else {
    let armadura = prompt("\nVOCE SE FERIU MUITO.")
}

if (capacete == 1) {
    let capacete = prompt("\nVocê se protegeu muito bem com o seu capacete.".toUpperCase())
} else {
    let capacete = prompt("\nVocê acabou sofrendo sem o seu capacete.".toUpperCase())
}

if (po_magico == 1) {
    let amu = prompt("\ngrandes habilidades adiquiridas com o po magico".toUpperCase())
} else {
    let amu = prompt("\nvoce foi a luta sem receber habilidades importantes".toUpperCase())
}

if (personagem == 1) {
    if (governo == 1) {
        let governo = prompt("\ O governo foi de grande ajuda".toUpperCase())
    } else {
        let governo = prompt("\Você não teria chegado tão longe sem ajuda do governo".toUpperCase())
    }
} else {
    if (governo == 1) {
        let governo = prompt("\as coisas complicaram sem a ajuda do governo".toUpperCase())
    } else {
        let governo = prompt("\nÉ muito difícil finalizar uma jornda desse tipo sem companhia.".toUpperCase())
    }
}

if (personagem == 1) {
 if (pontuacao == 0) {
    console.log(`\nOS LAGARTOS GANHARAM A GUERRA! A POPULACAO SOFRE.`)
 } else if (pontuacao == 1 || pontuacao == 2) {
    console.log(`\nOS LAGARTOS GANHARAM A GUERRA, A .`)
 } else if (pontuacao == 3) {
    console.log(`\nVOCÊ CONSEGUIU DETER OS LAGARTOS, MAS INFELIZMENTE NÃO SOBREVIVEU À BATALHA.`)
 } else if (pontuacao == 4) {    
    console.log(`\nAPESAR DE TER SIDO UMA BATALHA DIFÍCIL, VOCÊ CONSEGUIU DETER TODOS OS LAGARTOS!`)
 } else if (pontuacao == 5) {
    console.log(`\nVOCÊ CONSEGUIU DETER OS LAGARTOS, SALVOU SUA CIDADE E SE TORNOU UM HERÓI. SUA HISTÓRIA SERÁ LEMBRADA POR VÁRIAS GERAÇÕES!`)
 }
} else {
  if (pontuacao == 0) {
    console.log(`\nVOCÊ NÃO CONSEGUIU CHEGAR NEM PERTO DE DETER OS LAGARTOS.`)
 } else if (pontuacao == 1 || pontuacao == 2) {
    console.log(`\n A GUERRA FOI GANHA PELOS LAGARTOS.`)
 } else if (pontuacao == 3) {
    console.log(`\nVOCÊ CONSEGUIU DETER OS LAGARTOS, MAS NÃO SOBREVIVEU A ESSA GUERRA.`)
 } else if (pontuacao == 4) {    
    console.log(`\nTIVEMOS GRANDES PERDAS,A POPULACAO SOFREU, MAS VOCÊ CONSEGUIU DETER TODOS OS LAGARTOS !`)
 } else if (pontuacao == 5) {
    console.log(`\nVOCÊ CONSEGUIU DETER TODOS OS LAGARTOS, SALVOU A TERRA, VOCE E UM GRANDE HEROI!`)
 }   
}
