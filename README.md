# RegRipper3.0

Aqui está o que há de novo nesta versão

## O QUE HÁ DE NOVO:

- Com a Interface Gráfica (`rr.exe`), você não precisa mais selecionar um `perfil;`. Em vez disso, selecione a seção para analisar e o diretório de saída e a GUI serão executar automaticamente todos os plug-ins aplicáveis ​​no hive. Esse recurso é incluído no `rip.exe`, também, através da opção `-a`. Alternativa, você pode usar a opção `-aT` para executar todos os plug-ins TLN específicos do hive contra a colméia. A capacidade de executar plug-ins individuais, bem como perfis, também foi mantido. Você pode ver outras opções disponíveis digitando `rip` ou `rip -h` ou `rip /?` na linha de comando.

- Formato de data - Houve um problema no GitHub postado, solicitando que o formato de data fosse alterado para IAW [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601). No entanto, o formato real fornecido como parte do problema/solicitação foi IAW o perfil RFC 3339 (ou seja, espaço entre a data e tempo).


### OBSERVAÇÃO:

Esta ferramenta NÃO processa logs de transação do Hive automaticamente. Se você precisar para incorporar dados de logs de transações Hive em sua análise, considere mesclar os dados via `yarp` + `registryFlush.py` de Maxim Suhanov, ou via `rla.exe` de Eric Zimmerman que está incluído no [Eric's Registry Explorer/RECmd](https://f001.backblazeb2.com/file/EricZimmermanTools/RegistryExplorer_RECmd.zip).

Os seguintes arquivos de módulo Perl foram modificados e as versões modificadas são fornecido como parte deste repositório:

```cmd
C:\Perl\site\lib\Parse\Win32Registry\WinNT\File.pm
C:\Perl\site\lib\Parse\Win32Registry\WinNT\Base.pm
C:\Perl\site\lib\Parse\Win32Registry\WinNT\Key.pm
```

Se você estiver usando a versão Windows `exe` das ferramentas, isso é irrelevante, pois o os arquivos modificados são "**compilados**" no `exe`. No entanto, se você estiver instalando no Linux, copie os arquivos do repositório para os locais apropriados em sua instalação.

