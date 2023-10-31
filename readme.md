### Liguagens Quanticas

Esse é um repositorio onde gostaria de compartilhar as descobertas realizadas, na inciação cientifica que participei. 

Primeiramente precisamos entender que a computação quantica não é realmente aquele bicho de sete cabeças que muita gente acredita, mas obviamente é necessario tirar um tempo para  dedicar aos estudo e nesse repositorio é mais uma resumida de todo o estudo realizado, caso queiram saber mais podem ler os artigos que esse estudo gerou.

* <a href=''>Fatec-Seg</a>
* <a href=''>SICT</a>
* <a href=''>Revista fatec Americana</a>

O estudo foi realizado com base nas linguagens, <b>Silq</b> e <b>OpenQasm</b>, sendo a linguagem Silq uma linguagem de alto nível e a OpenQasm de baixo nível ambas são linguagens quanticas que são possiveis a criação de experimentos como por exemplo de algoritmos focando na criação de circuitos quãnticos. Antes de criar qualquer circuito ou tentar entender um codigo escrito em uma dessas duas linguagens, recomedo que leia sobre as portas que são possiveis aplicar.

### OpenQasm

Ela é a linguagem de baixo nível, que podemos utilizar na platafoma da <a href=''>IBMQ</a>, para se fazer possivel a execução dos circuitos, sendo no momento o lugar mais intuitivo para os estudos e experimentnos com essa linguagem, o OpenQasm é bastante parecido com o Assembly.

### Instalaçâo para a utilizar o SILQ

Esse é um tutorial em portugês que ensina como instalar e utilizar a linguagem silq na sua maquina!

* Silq é uma linguagem de programação de alto nivel para a computação quântica, que foi desenvolvida pela ETH Zürich.

* A maneira mais recomendada para instalar o silq é utilizando a extensão do Visual Studio code

* Antes de começar a utilizar o silq, vai ser necessario a instalação do  <a href="https://code.visualstudio.com/download">Vscode</a>.

<strong>Instalação da extensão</strong>

  <strong>1ª</strong> Abrir o Vscode.<br>
  <strong>2ª</strong> Abrir a guia de extensões e procure por <u>vscode-silq</u>.<br>
  <strong>3ª</strong> Baixar a extensão.
  <strong>4ª</strong> Importe a extensão para o vscode, da seguinte maneirta:
  * Vá na aba de extensões
  * Procura pelos (...)  acima da barra de pesquisa
  * Ao fazer o click, vai aparecer alguns campos e tem que pprocurar o <strong>Install from VSIX</strong>
  * Vá até a pasta onde baixou o arquivo e importe ele.
  
  <strong>4ª</strong> Comece a utilizar a linguagem silq.
  * Para rodar o codigo, salve e presione F5 ou F6 para fazer o debugg da aplicação

Caso não ache a extensão ou não consiga baixar é possivel realizar a instalação de outra maneira.

* Baixe a extensão como um arquivo <strong>.vsix</strong>.
* <a href="https://marketplace.visualstudio.com/items?itemName=eth-sri.vscode-silq">Download do arquivo</a> observe os Resources e clique em Download Extension e vai fazer o download automaticamnte.
* Abra o Vscode, vá na guia de extensões e clique nos três pontos no canto superior direito (<strong>...</strong>).
* Selecione a opção instalar do VSIX.
#
  ### Introdução básica
Para conseguir rodar um codigo Silq inicialmete começamos deixamos claro uma <strong>def</strong>, como por exemplo uma main para colocarmos o codigo dentro dela e ficaria assim um exemplo.

```silq
def main(){
    circ1:=0:B;
    circ2:=1:B;
    circ1:=H(circ1);
    return measure(circ1, circ2)
}
```

Onde aqui o codigo faz uma medição do circuito que aplicamos a porta de <strong>Hadamard</strong>, ele retorna o resultado que pode ser tanto que o circuito que aplicamos a porta volte como 1 ou 0 dependendo de qual polo estevesse mais proximo.
