---
title: "Backup com BootMii"
---

{% include toc title="Sumário" %}

O BootMii permite o backup e a restauração da NAND do seu Wii. Esta página irá guiá-lo no backup da sua NAND de Wii para um cartão SD, que você pode usar como preferir.

Wiis "Family Edition" (Wiis sem portas GameCube) NÃO PODEM restaurar backups da NAND. Isso ocorre devido à falta de portas GameCube que são necessárias em Wiis sem boot2 para entrar no código de confirmação de restauração. Seja como for, ainda se recomenda que se faça um backup nestes consoles.
{: .notice--danger}

Você precisa de um **cartão SD** para usar o BootMii, especialmente para criar um backup da NAND. Se você não tem um cartão SD na mão agora, você pode pular esta página, mas é ALTAMENTE RECOMENDADO voltar a esta página mais tarde para fazer um backup da sua NAND.
{: .notice--warning}

Navegar pelo BootMii não é possível usando um Wii Remote. Você deve usar os botões POWER e RESET em seu console, ou um GameCube plugado na porta 1. Para navegar entre as opções, pressione POWER no seu Wii (ou esquerda/direita em um controle de GameCube). Para selecionar uma opção, pressione RESET no seu Wii ou A no seu controle de GameCube. Você PRECISA usar um controle de GameCube para restaurar um backup da NAND no futuro se o BootMii estiver instalado como IOS.
{: .notice--info}

Se o botão `Launch BootMii` não aparecer no Homebrew Channel, [reinicie o Instalador HackMii](hackmii) e instale o BootMii.
{: .notice--warning}

Se a tela permanecer preta e a luz azul do disco piscar ao iniciar o BootMii, você não possui os arquivos do BootMii no seu cartão SD. Baixe [esse arquivo zip](https://static.hackmii.com/bootmii_sd_files.zip) e extraia ele para a raiz do seu cartão SD, então, tente novamente.
{: .notice--warning}

### Requisitos

* Um cartão SD com no mínimo 512MB de espaço livre (1GB ou mais é recomendado)

### Instruções

Se você tem o BootMii instalado como boot2, você precisará iniciar o BootMii reiniciando o console. Pule os passos 1 e 2 se for esse o caso.
{: .notice--info}

1. Ligue o seu console.
1. Abra o Homebrew Channel.
1. Pressione o botão HOME, depois selecione "Launch BootMii".

    ![](/images/bootmii/BootMii_Main.png)

1. Selecione o botão Opções (o ícone com as engrenagens).

    ![](/images/bootmii/BootMii_Gears_Icon.png)

1. Selecione o primeiro botão à esquerda.
    + Um backup da NAND será iniciado. Você pode assistir o progresso na tela.
    + "Bad Blocks" são normais, e a maior parte deles são originários de fábrica devido à ligação da NAND. Não se preocupe quando ver alguns deles em um backup da NAND.
    + Após este passo, ele irá verificar o backup. Idealmente, todos os blocos devem ser verdes após o processo de verificação.

    ![](/images/bootmii/BootMii_Green_Arrow.png)

1. Quando o processo estiver concluído, saia da tela de backup da NAND pressionando qualquer botão.

    ![](/images/bootmii/BootMii_NAND_Backup.png)

1. Pressione o botão Voltar (o botão com uma seta), então pressione o botão de Menu do Wii ou o botão do Homebrew Channel para sair do BootMii.

    ![](/images/bootmii/BootMii_Return_Arrow.png)

<div id="restore-notice" class="notice" markdown="1">
Nota: **restaurar um backup da NAND é geralmente a última coisa a se fazer**. Muitas vezes, existem maneiras melhores de desbricar seu console.
Tente o seu melhor para [identificar sua condição de brick](bricks) e reverter a ação que a causou em primeiro lugar.
Para restaurar de um backup da NAND no seu cartão SD, você pode seguir as instruções para a [RestoreMii](bootmiirecover) (Apenas Wii original).
</div>

Dois arquivos serão criados na raiz do seu cartão SD: `nand.bin` e `keys.bin`. `nand.bin` é a memória interna do seu Wii, enquanto `keys.bin` são as chaves do console.
{: .notice--info}

[Continue para a Instalação do Priiloader](priiloader)<br> Priiloader adiciona uma segunda camada de proteção para brick, e é altamente recomendado mesmo com o BootMii instalado como boot2. É especialmente importante para os usuários do BootMii na IOS.
{: .notice--info}