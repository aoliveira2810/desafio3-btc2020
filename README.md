# desafio3-btc2020

Para utilizar os códigos, é preciso:
1) Ter instalado na máquina o Python e o Scrapy.
#verifica se o Python esta instalado
$ which python3

#que deve retornar algo como /usr/bin/python. Isso significa que o Python está instalado nesse endereço.
#Para instalar o Python 3, digite em um terminal:
$ sudo apt-get install python3

#(Opcional) Para instalar o gerenciador de pacotes pip, digite em um terminal:
$ sudo apt-get install python3-pip

#Yum
#Para instalar o Python 3, digite em um terminal:
$ sudo yum install python3

#(Opcional) Para instalar o gerenciador de pacotes pip, digite em um terminal:
$ yum -y install python3-pip

## para instalar o Scrapy pelo pip
The quick way:
$ pip install scrapy
#ou 
## para instalar o Scrapy pelo conda
#baixa o arquivo do site oficial anaconda .sh
#https://www.anaconda.com/products/individual
#abra o terminal onde se encontra o arquivo e execute o comando: 
$ bash Anaconda3-2020.07-Linux-x86_64.sh

#Tela de Configuração Python Anaconda
#Depois de executar o comando bash você começará a configuração do Anaconda. Antes de mais nada, você vai precisar concordar com o acordo de licença. Basta apertar Enter para continuar.

#Agora você vai ver os longos parágrafos do acordo de licença, e pressionando a barra de espaço diversas vezes o levará até o final do documento. Para aceitá-lo, #digite Yes e pressione Enter.
#Em seguida, você deve definir o local onde o Anaconda Python deve ser instalado no seu Ubuntu. A localização padrão é o diretório HOME, e recomendamos que a #instalação seja feita aqui. Simplesmente pressione Enter para confirmar a instalação no diretório padrão ou defina manualmente um novo diretório para instalação.
#Finalmente, você irá ver que a instalação terá sido iniciada. Aguarde alguns minutos para que o processo seja finalizado com sucesso.

#Depois de a instalação do Anaconda Python ter sido concluída, você será solicitado se deseja incluir a localização do Python Anaconda no caminho do Ubuntu 18.04. #Digite Yes  e aperte Enter.
#Reabra o terminal para ativar as mudanças feitas, e o Anaconda Python estará pronto no seu Ubuntu 18.04.

#Para instalar este pacote com conda, execute um dos seguintes:
$conda install -c conda-forge scrapy
$conda install -c conda-forge/label/cf201901 scrapy
$conda install -c conda-forge/label/cf202003 scrapy 

2) Salvar os arquivos do git na máquina.

Após seguir os passos anteriores, basta utilizar o seguinte comando no prompt de comando a partir da pasta onde os arquivos estão salvos:
```
scrapy runspider <nome do arquivo python> -t json -o <nome do arquivo json>
```
Exemplo: 
```
scrapy runspider Desafio3-Artigos.py -t json -o artigos.json
scrapy runspider Desafio3-Videos.py -t json -o Videos.json
```
  
### Observação:
Estes scripts vão salvar as informações dos vídeos e dos artigos em um único documento para cada tipo de dado. Como a orientação é fazer o upload um por um, então é preciso salvar cada objeto json em arquivos diferentes manualmente.
