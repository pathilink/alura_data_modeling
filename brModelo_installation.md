# Instalar brModelo

Obs: Java deve estar instalado.

Passo 1: instalar o VIM

```
sudo apt update
```
```
sudo apt install vim
```

Passo 2: acessar <http://www.sis4.com/brModelo/download.html> e baixar a opção brModelo.jar.

Passo 3: criar uma pasta "brModelo" no mesmo caminho Downloads e adicionar o arquivo baixado nela.

Passo 4: Clique com o botão direito do mouse sobre a pasta e selecione a opção para abrir com o terminal.

Passo 5: estando no local do arquivo no terminal, execute em sequência os comandos abaixo.

```
sudo mkdir /opt/brModelo
```
```
sudo chmod +s /opt/brModelo
```
```
sudo chmod 777 /opt/brModelo
```
```
sudo cp brModelo.jar /opt/brModelo/
```

Passo 6: crie um ícone para o aplicativo.
```
curl -o ~/brModelo.png -OL https://github.com/chcandido/brModelo/raw/master/src/imagens/logico.png
```
```
sudo mv ~/brModelo.png /opt/brModelo
```

Passo 7: crie o arquivo "brModelo.desktop" dentro da pasta "applications"
```
sudo vim /usr/share/applications/brModelo.desktop
```

Passo 8: copiar e colar o conteúdo abaixo no arquivo aberto.
```
[Desktop Entry]
Version=3.2
Name=brModelo
Exec=java -jar /opt/brModelo/brModelo.jar
Icon=/opt/brModelo/brModelo.png
Type=Application
Comment=The software for MER
Path=/opt/brModelo
Terminal=false
StartupNotify=true
Categories=Development;Education;
```

Passo 9: salvar as alterações feitas. No VIM, para salvar as alterações precisamos pressionar a tela dois pontos e digitar as letras "wq" em minúsculo
```
:wq
```

Depois das etapas acima, o aplicativo será criado e pode ser acessado pesquisando por "brModelo" no buscador da máquina.

Fonte: https://cursos.alura.com.br/forum/topico-nao-consegui-instalar-o-brmodelo-no-linux-241791

Plataforma online alternativa: https://www.brmodeloweb.com/lang/pt-br/index.html