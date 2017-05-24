# 1. Introdução
 
HexChat, lançado em 2010, é um cliente IRC (Internet Relay Chat) baseado em XChat.

IRC é um protocolo de comunicação utilizado na internet, usado basicamente como bate-papo e troca de arquivos, permitindo assim a conversa em grupo ou privada. Foi documentado formalmente pela primeira vez em 1993, no documento RFC 1459 e suas subsequentes atualizações nos anos seguintes.

Já o XChat, lançado em 1999, também é um cliente IRC com uma GUI (Graphical User Interface) onde tem uma janela básica de bate-papo e algumas funcionalidades básicas encontradas em outros clientes IRC. Porém, esse software atualmente encontra-se descontinuado, sem nenhuma nova versão desde 2010 - a última versão é 2.8.9 - e nenhum patch/commit para seu código-fonte principal desde 2013.

A partir da versão 2.4.0 do XChat, seu principal desenvolvedor, Peter Železný, tornou o seu código proprietário no Windows. Especificamente, a versão para Windows passou a ser shareware que, após 30 dias de uso gratuito, requer o pagamento de uma taxa única de $19,99 dólares para registrar o programa. Isso foi feito para compensar o tempo gasto por Peter para atender a demanda de ter uma versão para Windows do XChat, originalmente um aplicativo GTK feito para Unix/Linux, uma tarefa considerada tediosa, tendo em vista que, entre Windows e Linux, existem diferenças no que se refere a forma de integrar a aparência e o comportamento do XChat no sistema operacional em questão.

Essa mudança para uma licença dupla - shareware no Windows, software live no Linux - gerou controvérsia e acusações de violação de direitos autorais. Entretanto, como a versão Linux do código do XChat ainda é código aberto sob a licença GPL v2 (GNU General Public License versão 2), alternativas gratuitas não-oficiais, inclusive para Windows, são mantidas e podem ser modificadas e distribuídas como quiser, desde que sigam a GPL. Dentre estas versões, está o HexChat (na época XChat-WDK), que é código aberto em todas as plataformas para as quais está disponível.

Inicialmente, HexChat foi chamado de XChat-WDK, tendo sido desenvolvido em 2010 apenas na plataforma Windows, ano no qual o XChat ainda estava sendo utilizado na plataforma Linux. A ideia inicial do então XChat-WDK era que pudesse unir com o XChat funcionando então para ambas as plataformas, porém o XChat teve seu desenvolvimento descontinuado. Então, a mudança de nome se fez necessária já que  WDK significa o Windows Driver Kit, portanto, não fazia sentido usar um nome específico do Windows para um aplicativo onde a intenção era que rodasse multiplataforma.

Escolheu-se o nome HexChat por ser escrito e pronunciado de forma quase idêntica a seu predecessor, o que foi considerado um bom nome para um novo começo.
 
![](https://hexchat.github.io/img/screenshot-windows.png)  
Figura: Janela do programa no Windows 8. Note pelo canto esquerdo que, em cada rede, pode-se conectar a múltiplos canais.
 
## Características

* Interface
 
É possível colocar a interface personalizada da maneira como o usuário deseja, disponível tanto para Windows quanto para Linux o download arquivos de temas personalizados, sendo que o gerenciador de temas é um aplicativo opcional incluído no instalador do Windows e compilável para Unix.

As cores das mensagens enviadas podem ser alteradas assim como sua formatação, podem ser alterados em Configurações >> Eventos de texto ou usando o seguinte código abaixo para ser formatado (lembrando sempre de pressionar o enter depois de editar um campo):
* % C <fg>, <bg> Código de cor (por exemplo,% C02,00 é azul sobre cinza)
* % R Cor inversa
* % U Texto sublinhado
* % B Texto em negrito
* % I Texto em itálico (2.10.0+)
* % H Ocultar texto
* % O Texto normal
* %% Escaped%
* $ T Separador de texto (caractere de tabulação)
* $ AXXX Valor de Ascii
* $ <Num> Informações do evento

Para personalizar mais do que apenas a cor do texto, como as bordas da janela, deve instalar um tema do gtk. O único requisito para temas no Windows é que eles são para gtk2 e eles usam o mecanismo Pixbuf. Os temas que exigem outras configurações funcionarão, mas não irão parecer corretos. Esta configuração porém só está disponível na release 2.10.0. Se você usar  uma versão abaixo da 2.12.0, precisará instalar o HexChat com a opção de tema Gtk desmarcada, isso evitará que o instalador a substitua nas atualizações.

Os temas podem ser instalados globalmente (alterando todos os aplicativos do gtk2) ou para o HexChat em específico. Este último requer permissões de escrita para o diretório de instalação do HexChat (por exemplo, em Arquivos de Programas). Os temas globais são definidos em % USERPROFILE% \.Gtkrc-2.0.

* Disponível nas plataformas Windows, OS X  e Unix, programado em C.
* Traduzido para vários idiomas

Podemos verificar no site https://www.transifex.com/hexchat/hexchat/ a evolução da tradução do sistema, abaixo o gráfico mais atual, de 2017.

![](https://lh6.googleusercontent.com/h3l99u2kHF7D1oNaq7JgVi96HzpXT8MzghKmiC5Kvg8WL3kpE3xK93K6dxxLOiiVukhbfkKvuEti4sMH9cM9e1nmCdhWJs5en6xdGVUZshLnqI0NuNicQTPtCENNq7WrrSGapq8)

![](https://lh3.googleusercontent.com/TyyaoGuLFqTFSek5Q7rn1ex1uXdho6i42uooaiqYnvm9GjOC9z57zQgLaB2PWHqkav417uw9WAFA7zfKj_C854W9XII3FlKCWhjZk8wO71lDhM1-6RW1-ogIuJZMHBYjxYOuj-A)
 
* Sistema totalmente open source.


# 2. Equipe de desenvolvimento
 
Atualmente 21 desenvolvedores contribuíram para o HexChat. Ao longo de toda a história de seu desenvolvimento, o HexChat teve 118 desenvolvedores. A imagem abaixo mostra os principais desenvolvedores da equipe, dentre os quais destacam-se Berke Victor e TingPing. A função de cada um na equipe não é informada.

![](https://lh6.googleusercontent.com/UA822dGirxf7pDHKtIwLyzScgHyfQzUFKA3EDQ2oG8bRR1if-K3CTccGZAf_2Ru17TZOlFC3tJb4QVzjwDm-kVV_9PktqmqiUPjnIEa3l3YpLrCeAb3MvgDnfdowUxKz1Byef3o)

![](https://lh3.googleusercontent.com/4q_8fDvFe4zY__flYmgZP9OKfXikZzl_0LK9eXZVq6Lg0nQxAnZV9RJ_ON-UrDftd1CZbJRIA_O-aptwWqmHN0Al6eYczva7Autrai73Nki1hcnKFEv4trH--fjz4baG4kWOcOg)

O gráfico abaixo mostra o número de contribuidores que o HexChat já teve, o maior número de contribuidores por mês foi em maio de 2013 com 12 contribuições.

![](https://lh4.googleusercontent.com/YCLW48AEvBV64A7kjPQEUmadB52L-_-jNbfKe3OmUabhViJwgwFNPqZt83lgBb6roIBt-ri0WljoqlnJmRD0YDEGgN7qNHi3sulzp8NFttoXdUJcIwgCxlFUYeHMW3WjtjcB4JM)


# 3. Evolução do sistema 
 
HexChat tem atualmente 3.279 commits feitos por 118 desenvolvedores, totalizando 72.876 linhas de código, escrito principalmente em C. As primeiras linhas de código fonte foram adicionadas em 2010, sendo de que desse número total 10% são comentários.
 
![](https://lh3.googleusercontent.com/8JNVTORuqOUk2ksv-24D0amq7EDemFV0GNdZSI2KY0Aifp0U5hC8L1qT9to8hXqdyGCaim1KPKWqyavkDjahkZIswrHMMIyRK8mJn0pzjaWlZbVdBeMui6WH637Bj8cJtXKcxNg)

![](https://lh3.googleusercontent.com/u41eUgXzg_cZBelyXH3e-mGRzsK7EyJZhNTh_YF3-24_XPh89nr7XEO2D2pKb7dvi6jX4fz0L4Z2HmRjSj_w_Shl9-F-EhXeUYBPG7Ghh3f4Hb4mpcUAkTw9POvI5a5Gt8SID0M)
 
A figura abaixo mostra o gráfico das principais linguagens de desenvolvimento do HexChat:
 
![](https://lh6.googleusercontent.com/bwjJYZwOURH4RHYIjs8bGwZN-zWDgA0faBV1Ws57z7wCPv_DZrnPYUd-asDPj7_OkcfgsfXegB5k6uD-IPSkNkcwTW22G1iUCk-V0JulEToruaUHT09OcuTQ8W7kIxygHy2DQJU)
 
## Principais releases
 
A release inicial foi a 1409, em 2010, e seguiu-se com este esquema de numeração até a release 1508-3, em 2012. A partir daí, teve a mudança não só do nome do programa, de XChat-WDK para HexChat, mas também da numeração de versões.

Como a última versão do XChat foi 2.8.9, HexChat resolveu alterar a numeração de suas releases, tal que a release 1515 passou a ser conhecida como versão 2.9.0. Foi a partir desta versão também que o código do programa foi migrado para o GitHub.

A última vez que a numeração de release foi usada foi para a release 1521, vulgo versão 2.9.1. Versões posteriores não teriam mais seus números de release listados no changelog.

A seguir, algumas dessas versões posteriores:
 
### Versão 2.9.4
 
Lançada em novembro de 2012, esta versão conta com um novo tema, suporte SASL construído e um plugin sysinfo no Linux. 
 
### Versão 2.9.5
 
Lançada em abril de 2013, esta versão não suporta mais o Windows XP e vem com mudança na correção ortográfica. O download, antes realizado pelo GitHub, deve ser feito agora diretamente do site do HexChat.
 
### Versão 2.9.6
 
Lançado em setembro de 2013, essa versão conta com o suporte SASL expandido para incluir a criptografia BLOWFISH e AES e EXTERNAL para uso de certificados no lado do cliente. Correção de bugs e suporte para script em Python.
 
### Versão 2.10.0
 
Lançada em junho de 2014, esta versão não teve uma alteração muito grande com relação a anterior, apenas correção de alguns bugs e agora oferece suporte para OS X, além de algumas melhorias na UI e na caixa de entrada e pesquisa.
 
### Versão 2.10.2
 
Lançada em novembro de 2014, esta versão melhorou a segurança do envio de mensagens. Agora, os nomes de host são verificados, bem como algumas outras opções mais seguras. Houve também uma mudança na hospedagem dos downloads.
 
### Versão 2.12.0

Lançada em março de 2016, esta versão, além da correção de bugs, é relatado um esforço por parte dos desenvolvedores para que as funcionalidades do sistema sejam iguais em todas as plataformas, como notificações e verificação ortográfica. Vários plugins foram completamente reescritos a partir do zero para corrigir problemas e melhorar o suporte a plataformas cruzadas. Nessa versão, o plugin de atualização permite uma caixa de diálogo de atualização gráfica mostrando o log, conforme imagem a seguir:
 
![](https://lh4.googleusercontent.com/Ez4O8yRygvzs1yqCsFPTCAPvGeVFBdEve4lU_Buz-WoMYHPBFLXl6kR3SwvUqSUaGR9IYhekWbCmDf8yPUjrw110WUemSQJ9YLOpQCzFWCdfa0PZnyla-hcqUiuu60Iy7zUhOxg)
 
### Versão 2.12.1

Lançada em maio de 2016, esta versão, além da correção de bugs, agora é permitido scripts em Lua. A linguagem Lua é extremamente portátil e sendo assim os usuários do Windows não precisam baixar o instalador de Python.

Agora também é possível usar uma biblioteca chamada lgi .GObject-Introspection é uma tecnologia que permite que informações sobre bibliotecas C sejam usadas externamente (geralmente de outros idiomas). Isso significa que os scripts podem se integrar com as mesmas bibliotecas que HexChat usa em si, como GLib e Gtk. Esta biblioteca é pequena o suficiente para que possamos agrupá-la no Windows, o que significa que, pela primeira vez, todos os usuários do Windows podem ter scripts que podem modificar facilmente a interface do usuário ou integrar com o mainloop.
 
### Versão 2.12.2

Lançada em outubro de 2016, esta versão não teve grandes mudanças, tendo apenas corrigido os bugs encontrados na versão anteriormente lançada.


# 4. Características de desenvolvimento
 
As versões do HexChat disponíveis atualmente são para as plataformas Windows e Linux. Windows possui um modo portátil que requer que os seguintes componentes sejam obtidos manualmente:
 
* Visual C++ 2015 Redistributable
* Dicionários para verificação ortográfica (necessário apenas para Windows 7)
* Python 2.7.12 para scripts
* Python 3.5.2 para scripts 
* Perl 5.20.0 para scripts
 
Caso a instalação não seja em modo portátil, o instalador baixa estes componentes automaticamente.
 
Versões para Mac/OS X não são mais mantidas no site oficial, mas HexChat ainda pode ser instalado nessa plataforma através de dois recursos: Homebrew, o mais simples e automático; e JHBuild, que é uma alternativa mais complexa.
 
HexChat é um software livre sob a licença GPL v2, tendo como exceção a permissão de uso, compilação e/ou linkagem do OpenSSL. Pode-se prover pacotes binários ligados as bibliotecas do OpenSSL, desde que os outros requisitos da GPL sejam seguidos.
 
## Addons
 
HexChat possui alguns plugins úteis que estendem a funcionalidade do cliente. Para carregar plugins personalizados automaticamente, eles devem ser colocados no subdiretório de addons dentro do seu diretório config, seja manualmente com /load e /unload, ou em Window ‣ Plugins and Scripts.
 
![](https://lh3.googleusercontent.com/DfN6U7eZ8Vxx7TRTaYWZdUN1Kw0IPnWkCCJCy-mtQ3-c6WatHKw3PfO8G-KB9akHhTpAE_unvzTVEqdEceVZbFq2-Eye7qByLSiu5PMT-X21Hvg7vZuR81skrqIUYxDneTlQfFM)  
Figura: Janela de plugins e scripts após uma instalação padrão do HexChat
 
Com as interfaces de script incluídas, pode-se usar scripts mais fáceis de criar, porém igualmente poderosos em linguagens como Python. Estas são (des)carregadas da mesma maneira que plugins.
 
### Exec

Provê o comando /exec para Windows, já está compilado no Unix.

Com Exec, pode-se executar comandos como se estivessem sendo executados pela linha de comando. A saída será impressa imediatamente, ao final da execução. Se o comando levar mais de 10 segundos para completar, ele é abortado para evitar o travamento do HexChat. Exemplo: 
/exec ping google.com
 
### FISHLiM

Adiciona suporte a criptografia FiSH. Configura-se uma senha para uma conversa/canal e então todas as suas mensagens são criptografadas. Apenas os que sabem a senha poderão ler suas mensagens.

Uso é simples. Primeiro, configure a senha: 
/setkey yoursecretkey

Então informe os participantes da conversa sobre esta senha. Assim que eles também configurarem a senha do lado deles, eles receberam mensagens descriptografadas e enviá-las criptografadas também.

A chave pode ser removida com: 
/delkey #channel
 
### Update Checker

![](https://lh5.googleusercontent.com/A2P19ZYBJ0mF3VMlP636j7_T7RI-BkAU0PU8fGmQvKuIZVVemRXZvX6mTN1RdyiTiHaXDoKeJEOwgIxb6dzlqV6_gJDHvwcRWaW0V8xrZsmFCuPtY6Co5Wc88u-bFe4PSWwsR3M)  
Figura: Verificação de atualizações
 
Verifica automaticamente por atualizações disponíveis. Pode ser ativado manualmente via Help ‣ Check for Updates ou pelo comando: 
/updchk
 
### Sysinfo

Imprime informação de sistema básica tanto em Windows como em Unix. Pode ser ativado em Window ‣ Display System Info ou digitando: 
/sysinfo
 
### Checksum

Calcula automaticamente o checksum SHA-256 de arquivos enviados e recebidos via DCC.
 
### Winamp

Exibe o áudio sendo reproduzido no momento via Window ‣ Display Current Song ou pelo comando: 
/winamp
 
Nota: Foobar2000 também pode ser usado com o plugin foo_winamp_spam.


# 5. Arquitetura
 
## Código principal
 
Por se tratar de um software derivado do XChat, escrito primariamente em C, a organização do código-base se dá em estruturas de dados ao invés de objetos. O código-fonte principal em C encontra-se no diretório /src, principalmente nos subdiretórios /common e /fe-gtk. Segue abaixo o mapa de alguns dos principais arquivos:
 
### Subdiretório /common:
 
* hexchat.c - Principal arquivo do programa, contém main()
* hexchat.h - Principal arquivo de header, contém a maioria dos structs mais importantes usadas no HexChat
* outbound.c - Código para lidar com comandos
* inbound.c - Código para lidar com dados do servidor
* text.c - Código para logging e lidar com texto
* plugin.c - Todo o código de plugin
 
### Subdiretório /fe-gtk:
 
* editlist.c - Código genérico para lidar com listas editáveis (como a lista Userlist Buttons)
* fkeys.c - Lida com chaves de funções
* gtkutil.c - Wrappers ao redor do GTK (a interface gráfica)
 
A documentação oficialmente divulgada do Hexchat, no que se refere a estruturação e detalhamento do código, é mais voltada para a interface de plugins e scripts, por isso não trata do restante do código-base interno.
 
No entanto, existe uma configuração do Doxygen para gerar esta documentação a partir do código-fonte do sistema escrito em C que, embora praticamente não é usada nem mantida pela comunidade, oferece uma outra visão de como os arquivos em C estão estruturados.
 
A saída gerada pelo Doxygen (em HTML) para o HexChat pode ser obtida aqui: https://www.dropbox.com/s/4h1kq5m71dlkqkq/hexchat-html.tar.xz
 
Segue na imagem abaixo o índice de classes C do HexChat encontradas pelo Doxygen:
 
![](https://lh4.googleusercontent.com/YY269u-JXuSHWJ5DsXr_X14Teq91LRhuHMpHO5W3WNF4nN3HCYgTDhfxBhSK_8oirDPAaotydx6erxSIbyifZsKkRthd71WMG1CF_mqaOMZnGRMibNCm_o2lqPfxmp7iiNQxFT0)
 
Dentre os arquivos de saída gerados pelo Doxygen, pode destacar-se também a geração de grafos de chamadas para as funções em arquivos SVG, dentre elas a da função main() exibida abaixo (no formato PNG):
 
![](https://lh3.googleusercontent.com/9Y9Pvocud2wt3lD56HJHd9zbXAqPUymQHgGpcBBq-z9M7SlEmGV5GVgSTcYyzWdOVSaDysLt1LcmR4Un1cnSoLsPkn-c3sRliHHsTC7tAof6JIxzqAtkxDg2I8nPwIjUCF4ys-I)
 
## Scripts e plugins
 
Scripts originalmente escritos para XChat geralmente são compatíveis com pequenas modificações, enquanto plugins binários geralmente precisam ser recompilados especificamente para HexChat.
 
### Plugins
 
HexChat tem a mesma arquitetura de plugins binários do XChat e estes plugins são usados para carregar interpretadores para linguagens de script comuns no cliente. Módulos são providos para JavaScript, Lua, Perl e Python. Um plugin para suporte a Tcl originalmente estava disponível, mas não é mais mantido. Existe também um plugin D-Bus que possibilita desenvolver programas externos que podem controlar o cliente.

Plugins para HexChat são escritos em C. A interface tem como objetivo possuir compatibilidade binária total, o que significa que, ao atualizar HexChat, não será necessário recompilar plugins pois eles continuarão funcionando. A interface não depende de qualquer estrutura nem de offset, então versões de compilador não devem ser afetadas também.

O único requisito de um plugin para HexChat é a definição de uma função hexchat_plugin_init, pois ela é o ponto de entrada. Todas as funções e variáveis globais devem ser estáticas, para que não sejam exportadas. Não há perigo nesta exportação, mas ela não é necessária e apenas polui o espaço de nomes. Plugins são compilados como objetos compartilhados (arquivos com extensão .so). Por exemplo:
 
* Maioria dos sistemas UNIX: 
gcc -Wl –export-dynamic -Wall -O1 -shared -fPIC myplugin.c -o myplugin.so
 
* OS X: 
gcc -no-cpp-precomp -g -O2 -Wall -bundle -flat_namespace -undefined suppress -o myplugin.so myplugin.c
 
No Windows, plugins são compilados pelo Visual Studio. Recomenda-se usar um plugin existente como ponto de partida. Feito isso, usa-se os seguintes arquivos:
 
* hexchat-plugin.h - principal header domain plugin
* plugin.c - seu plugin
* plugin.def - um simples arquivo de texto contendo o seguinte (hexchat_plugin_deinit é opcional):
 
EXPORTS
hexchat_plugin_init
hexchat_plugin_deinit
hexchat_plugin_get_info
 
Daí, basta compilar o plugin no Visual Studio normalmente.
 
Todas as strings passadas de e para plugins são codificadas em UTF-8, independente da localidade.
 
### Scripts
 
As integrações com Perl e Python requerem que o interpretador apropriado seja instalado - normalmente, usuários Windows terão que instalá-los e usuários Unix/Linux já os tem disponíveis.

Existem múltiplas linguagens de scripts suportadas por HexChat, mas atualmente apenas Python (versões 2.7 e 3.5), Perl (versão 5.20) e Lua são oficialmente suportadas, Lua sendo a opção recomendada.
 
Já existe uma documentação extensiva (em inglês) para várias interfaces de script, então elas não serão tratadas em maiores detalhes aqui.
