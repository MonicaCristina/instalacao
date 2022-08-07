<h1>Instalando as IDEs Java </h1>

<p> 🚦 Guia </p>

<h2><strong> 🐧 LINUX</h2></strong>

<h3>🔺 Instalação OpenJDK</h3>

<em><strong>O OpenJDK (Kit de Desenvolvimento Java Aberto)</strong> é uma  implementação gratuita e de código aberto da linguagem de programação  Java.  A implementação está licenciada sob a GNU General Public License  (GPL) com uma exceção de vinculação. <strong>JDK = JRE + JVM</strong></em>

🔸 <strong>1.</strong> Abra o terminal e vamos verificar se temos o Java instalado:

```
java -version
```

🔸 <strong>2.</strong> Para instalar o openJDK-11, digite no terminal:
<em>A versão mais atual LTS é do Java 11, que terá seu suporte  estendido até Setembro de 2022. Este tipo de suporte iniciou no Java 8  que será mantido até 2023.</em>

```
sudo apt-get install openjdk-11-jdk
```

🔸 <strong>3.</strong> Confirme se realmente foi instalado com sucesso:

```
java -version
```

🔸<strong>4.</strong> Vamos configurar o ambiente JAVA_HOME:

​	<strong>4.1</strong> Verificar o caminho da instalação do Java:

```
sudo update-alternatives --config java
```

​	<strong>4.2</strong> Copie o caminho que aparecerá no terminal, no meu caso:

```
/usr/lib/jvm/java-11-openjdk-amd64/bin/java
```

​	<strong>4.3</strong> Vamos editar o arquivo .bashrc:

```
sudo gedit ~/.bashrc
```

​	<strong>4.4</strong> Copie o código abaixo e cole no final do arquivo .bashrc. 

​	<em>IMPORTANTE: cuidado para não alterar nada no arquivo além de apenas colar no final do mesmo o que vou te disponibilizar a seguir. </em>

​	<em>JAVA_HOME = aqui você coloca o caminho do tópico 4.2, tirando o /bin/java</em>

```
JAVA_HOME=/usr/lib/jvm/java-11-openjdk-amd64
export JAVA_HOME
export PATH=$PATH:$JAVA_HOME
```

​	<strong>4.3</strong> Salve o arquivo

​	<strong>4.4</strong> Vamos conferir se a alteração ficou salva:

```
cat ~/.bashrc
```

🔸<strong>5.</strong>  Feche o terminal e abra novamente

🔸<strong>6.</strong> Vamos conferir mais uma vez se o Java está instalado na nossa máquina

```
java --version
```


<h3>🔺 Instalação Eclipse </h3>

🔸 <strong>1.</strong> Entre no site oficial do Eclipse Foundation e faça o <strong><a href="https://www.eclipse.org/downloads/download.php?file=/oomph/epp/2021-06/R/eclipse-inst-jre-linux64.tar.gz">DOWNLOAD</a></strong>
<em>O site já identifica o sistema operacional.</em>

🔸 <strong>2.</strong> Descompacte a pasta

🔸 <strong>3.</strong> Procure o arquivo eclipse-inst e execute

🔸 <strong>4.</strong> Escolha segunda a opção: Eclipse IDE for Enterprise Java and Web Developers

🔸 <strong>5.</strong> Clique no folder da primeira opção e selecione o JDK que instalamos na nossa máquina.

🔸 <strong>6.</strong> Mantenha as opções "create start menu entry" e "create desktop shortcut"

🔸 <strong>7.</strong> Install

🔸 <strong>8.</strong> Accept now

🔸 <strong>9.</strong> Launch

🔸 <strong>10.</strong> Pronto, intalação concluída!

<br>

<h3>🔺 Configurando o ícone do Eclipse IDE no Dock </h3>

<br>

<h3>🔺 Instalação IntelliJ IDEA Community </h3>

🔸 <strong>1.</strong> Entre no site ofical do <a href="https://www.jetbrains.com/idea/download/#section=windows"><strong>INTELLIJ</strong></a>

🔸 <strong>2.</strong> Escolha a opção Community e faça o download 

🔸 <strong>3.</strong> Descompacte a pasta e vamos para o terminal

🔸 <strong>4.</strong> Abra o terminal (Ctrl + Alt +  t) e entre no diretório que você descompactou 
<em>No meu caso, na pasta Downloads Ideal</em>

```
cd Downloads/IdealC
```

🔸 <strong>5.</strong> Entre na pasta bin

```
cd bin
```

🔸 <strong>6.</strong> Execute o arquivo de instalação idea.sh

```
./idea.sh
```

<br>

<h3>🔺 Instalação Git </h3>

🔸 <strong>1.</strong> Abra o terminal (Ctrl + Alt + t) e vamos verificar se temos o git instalado:

```
git --version
```

🔸 <strong>2.</strong> Execute o comando:

```
sudo apt-get install git-all
```

🔸<strong>3.</strong> Confirme novamente se o git realmente está instalado:

```
git --version
```

🔸 <strong>4.</strong> Vamos começar as configurações iniciais:

​	<strong>4.1</strong> Cofigurar o nome de usuário

```
git config --global user.name "Seu nome"
```

​	<strong>4.2</strong> Configurar o endereço de e-mail:
​	<em>É de suma importância que o ENDEREÇO DE E-MAIL SEJA O MESMO DO GITHUB afim de evitar conflitos!</em>

```
git config --global user.email seuemail@email.br
```

​	<strong>4.3</strong> Vamos conferir a lista de configurações:

```
git config --list
```

🔸 <strong>5.</strong> Pronto, git instalado e configurado com sucesso!

<br><br>
