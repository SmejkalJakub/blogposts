Po několika různých nástrojích a přístupech ke správě, vyvíjení a flashování firmwarů jsme se rozhodli, že nejlepší cestou bude vyvinout vlastní Visual Studio Code rozšíření spolu s kompletní portable verzí, která obsahuje všechny potřebné nástroje.

Předchozí zkušenosti s rozšířením PlatformIO nás přesvědčili o užitečnosti Visual Studio Code, neměli jsme ovšem větší kontrolu nad rozšířením a proto došlo na naše vlastní rozšíření s názvem **HARDWARIO TOWER**.

Pokud využíváte VSCode již déle a nechcete se vzdát svého prostředí, je možné si stáhnout rozšíření ve formátu .vsix z [**našeho GitHubu**](https://github.com/hardwario/hardwario-tower-vscode-extension/releases). Více o tom jak nainstalovat rozšíření je možné nalézt [**v naší dokumentaci**](https://docs.hardwario.com/tower/firmware-development/tower-vscode-extension#installation). Nevýhoda této metody je, že si musíte nainstalovat všechny potřebné nástroje.

Pokud nemáte vlastní nastavený VSCode či nechcete instalovat potřebné nástroje, je možné využít naší Portable verze s názvem HARDWARIO Code. Tato portable verze obsahuje všechny nástroje potřebné k vývoji s HARDWARIO TOWER. Po jednoduché instalaci můžete rovnou začít vyvíjet. Více o této verzi opět v [**naší dokumentaci**](https://docs.hardwario.com/tower/firmware-development/about-hardwario-code).

Naše rozšíření obsahuje několik příkazů a funkcní pro zjednodušení práce s firmwarem a jeho vývoje. V dokumentaci je možné nalézt [**detailní popis jednotlivých funkcí a celého rozšíření**](https://docs.hardwario.com/tower/firmware-development/hardwario-extension-tutorial).

## Orientace v HARDWARIO Code

Po otevření HARDWARIO Code se na levé liště nachází **logo HARDWARIO**, po rozkliknutí tohoto loga budete mít přístup ke všem, momentálně dostupným příkazům.  

## Rychlé vytvoření nového projektu

HARDWARIO Code umožňuje vytvořit nový projekt z našeho **twr-skeleton** což je základní struktura TOWER firmwaru. Tento projekt jednoduše zklonujete z rozšíření stisknutím **From Skeleton Project...** v sekci **TOWER: Start**. Následně můžete zvolit rodičovskou složku projektu a popřípadě název.



Pokud již víte s jakými moduly budete pracovat popřípadě se chcete inspirovat již vytvořeným projektem, je možné použít **From Existing Project...** v sekci **TOWER: Start**, Zde budete moci vybrat název projektu, který vás zaujal a tento projekt si zklonovat.

Tento postup je detailněji popsán v kapitole [**Firmware Quick Start**](https://docs.hardwario.com/tower/firmware-development/firmware-quick-start)

## Upgrade starého projektu

Během let jsme ve stavebnici TOWER několikrát obměnili nástroje a způsoby sestavení firmwaru. Poslední změna nás vedla k použití CMake a Ninja. Pro zjednodušení tohoto přechodu je v HARDWARIO Code implementován systém pro upgrade jakéhokoli starého projektu, který můžete chtít znovu využívat s HARDWARIO Code. 

Stačí otevřít tento projekt v HARDWARIO Code či ve vašem VSCode s nainstalovaným rozšířením HARDWARIO TOWER. Po otevření budete upozorněni na zastaralý projekt s možností upgradu. Po krátké době by měl být projekt připraven na použití v novém prostředí.

## Flashování do Core Modulu

Pro zjednodušení procesu sestavení a flashování firmwaru je v HARDWARIO Code několik dostupných příkazů.

Firmware je možné sestavit či flashovat jednotlivými příkazy či je možné využít jeden příkaz, který provede celý proces krok po kroku od sestavení až po připojení k TOWER Konzole.

## TOWER Konzole

Součástí HARDWARIO Code je i integrovaná konzole, kterou je možné využít pro logování informací z připojeného Core Modulu či odesílání AT příkazů pro ovládání připojeného Core Modulu (pokud jsou AT příkazy podporovány firmwarem).