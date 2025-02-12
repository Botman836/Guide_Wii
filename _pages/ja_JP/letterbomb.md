---
title: "LetterBomb"
---

{% include toc title="Table of Contents" %}

For instructions on how to format your SD card correctly, please see [this guide](https://wiki.hacks.guide/wiki/Formatting_an_SD_card). It is highly recommended to check it due to problems with formatting as FAT32.
{: .notice--info}

Do NOT use any of the MAC address examples shown in this guide, as they will simply cause an error on the HackMii website. Use your own!
{: .notice--warning}

LetterBomb is an exploit for the Wii that is triggered using the Wii Message Board.

### 必要なもの
* An SD card formatted as FAT32
* A Wii on System Menu version 4.3
* A Windows/MacOS/Linux computer with an Internet connection

### 実行方法

1. Wiiの電源を入れます。
1. `Wii設定`に進みます。
1. バージョンを確認してください。1ページ目の右上に表示されています。
    + これはシステムメニュー領域に対応しており、後ほど実行する手順に必要となります。
    + Also, ensure that you are on System Menu version 4.3.

    ![](/images/wii/SystemMenuVersion.png)

1. Navigate to `Internet` > `Console Information`.
1. Take note of your FULL MAC address.

    ![](/images/wii/MacAddress.png)

1. On your computer, open the browser and go to [the HackMii website](https://please.hackmii.com/).
1. Input your Wii MAC address and region.
1. Ensure `Bundle the HackMii Installer for me!` is checked.
1. Cut either wire.

    ![](/images/exploits/letterbomb/LetterBomb-PC.png)

1. Insert your SD card into your computer.
1. Copy the `private` folder and the `boot.elf` file from the LetterBomb `.zip` to the root of your SD card.
1. Reinsert your SD card into your console.
    + The SD card must be inserted in the SD card slot located in the front of the Wii. Using a USB to SD adapter plugged into the Wii's USB port will not work.
1. On your Wii, return to the Wii Menu.
1. Launch the Wii Message Board.
1. Open the red letter with a bomb.
    + Ensure the date on your Wii is correct, otherwise you might be unable to find the letter.
    + In some cases, you may need to check the messages for tommorow or yesterday for the letter to show up.
    + If you don't see the red letter, check if any errors appear in the SD card section of `Data Management`. If any do, there may be an issue with the SD card format or the Wii’s SD card reader.
    + If your Wii freezes after clicking on the letter, you most likely chose the wrong system menu region for LetterBomb. Go back to Step 2 and verify that you chose the right region.
    + If all is correct and there is freezing, keep on trying until it works.
1. 成功すると、WiiはHackMiiインストーラーをロードします。

![](/images/exploits/letterbomb/LetterBomb-Wii.png)

[Continue to Homebrew Channel and BootMii Installation](hbc)
{: .notice--info}
