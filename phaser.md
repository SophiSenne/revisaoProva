# Questões Phaser

### Qual das opções abaixo cria um jogo Phaser com largura de 800px e altura de 600px?

```
const config = {
    type: Phaser.AUTO,
    width: 800,
    height: 600,
    scene: {
        preload: preload,
        create: create,
        update: update
    }
};
const game = new Phaser.Game(config);
```

x (A) Correto

(B) Falta definir a cena corretamente

(C) O Phaser não usa Phaser.AUTO

(D) A variável config deveria ser um array


### Como adicionar física a um sprite no Phaser 3?

```
function create() {
    const player = this.add.sprite(400, 300, 'player');
    // Código aqui
}
```
(A) this.physics.enable(player);

(B) this.add.physics(player);

x (C) this.physics.add.existing(player);

(D) player.enablePhysics();

### Qual código adiciona um teclado para capturar a tecla seta para cima?

```
function create() {
    this.cursors = this.input.keyboard.createCursorKeys();
}
function update() {
    if (/* Código aqui */) {
        console.log('Tecla pressionada!');
    }
}
```

(A) this.cursors.UP.isDown

x (B) this.cursors.up.isDown

(C) Phaser.Keyboard.UP

(D) this.input.keyDown('UP')

### Como adicionar um movimento de velocidade fixa para um sprite chamado player usando Arcade Physics?

```
function update() {
    // Código aqui
}
```
x (A) player.setVelocity(200, 0);

(B) player.velocity = 200;

(C) player.setSpeed(200);

(D) player.moveX(200);

### Como impedir que um sprite saia da tela?

```
function create() {
    player = this.physics.add.sprite(400, 300, 'player');
    // Código aqui
}
```
x (A) player.body.setCollideWorldBounds(true);

(B) player.enableBoundsCollision();

(C) player.setBoundsCollision(true);

(D) player.setWorldBounds(true);

### Como animar um sprite no Phaser?

```
function create() {
    this.anims.create({
        key: 'walk',
        frames: this.anims.generateFrameNumbers('player', { start: 0, end: 3 }),
        frameRate: 10,
        repeat: -1
    });
    // Código aqui
}
```
x (A) player.play('walk');

(B) player.animate('walk');

(C) player.startAnimation('walk');

(D) player.begin('walk');

### Qual dessas linhas de código inicia um temporizador para executar uma função após 5 segundos?
```
function create() {
    // Código aqui
}
```

(A) this.time.delayedCall(5000, () => console.log('Tempo acabou!'));

(B) setTimeout(() => console.log('Tempo acabou!'), 5000);

(C) this.timer.start(5000, () => console.log('Tempo acabou!'));

(D) this.schedule(5000, () => console.log('Tempo acabou!'));

### Qual é a principal vantagem de usar um physics engine como Arcade Physics no Phaser?

(A) Melhorar o desempenho do código JavaScript

X (B) Controlar colisões e movimentação de forma simplificada

(C) Criar animações mais rapidamente

(D) Melhorar a renderização de sprites