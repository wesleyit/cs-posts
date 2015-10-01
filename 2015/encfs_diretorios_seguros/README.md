
Está trabalhando naquele "super projeto" e anda preocupado com a segurança dos seus dados?

Faz todo sentido, afinal, a grande maioria dos desenvolvedores trabalha em um notebook.

Sexta-feira, voltando para casa, carro parado no semáforo e pimba! Perdeu, playboy! 
Além do incoveniente de perder os dados (podemos falar de estratégias de backup outro dia), imagina todo o seu código simplesmente "passeando" por aí?

Para evitar (ou pelo menos dificultar bastante) o acesso aos seus dados no HD, uma boa saída é criptografar seus dados.

No Mac OS X basta ativar o [FileVault](https://support.apple.com/pt-br/HT204837). No Windows também é fácil, ś só ligar o [Bitlocker](http://windows.microsoft.com/pt-br/windows-8/bitlocker-drive-encryption). No Linux também é fácil: com um clique, durante a instalação do Ubuntu, Debian, Fedora, OpenSuSE e muitas outras distribuições, é possível ativar a criptografia no diretório `home` ou até mesmo no disco todo.

Mas e se seu Linux já está instalado e você não usou criptografia? E se você quer criptografia apenas para uma pasta específica?
O Linux utiliza o LUKS como padrão para criptografia de disco. Através dos módulos DM-Crypt, inclusos no Kernel, e dos utilitários Cryptsetup, é possível configurar uma infinidade de cenários. O problema é que estes programas são complicados, a documentação não é tão clara e amigável, e problemas na configuração podem fazer a máquina parar de inicializar, sendo necessário reformatar o computador. Assustador, não é?

A alternativa que vamos mostrar hoje é o [eCryptFS](http://ecryptfs.org/about.html). eCryptFS é uma solução opensource e é utilizado como base para o sistema de criptografia de pasta de usuário no Ubuntu Linux e também no Google Chrome OS.

Como queremos facilidade, vamos utilizar uma ferramenta gráfica para gerenciar nossa pasta segura - mas vou mostrar como montar uma pasta via linha de comando também.

Vamos começar. Estou utilizando um Debian Jessie, mas os processos mostrados aqui são parecidos no Ubuntu e outras distros baseadas em Debian. Para outras distros, procure no seu gerenciador de pacotes.

```
root@e109c3ef5577:/# apt-get install -y encfs ecryptfs-utils
Reading package lists... Done
Building dependency tree       
...
root@e109c3ef5577:/#
```



Outras distribuições:
http://software.opensuse.org/download.html?project=home:moritzmolch:gencfsm&package=gnome-encfs-manager


