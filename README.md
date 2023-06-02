# curso-biblioteca-

Exemplo de aplicação de biblioteca gráfica
Você sabia que o desenvolvimento de jogos digitais é a atividade que mais faz uso das bibliotecas gráficas, realizando a interação com elementos gráficos, sejam eles 2D ou 3D?

Saiba então que se destacam dois conjuntos de bibliotecas gráficas: A OpenGL e a DirectX (que serão estudadas com maior detalhe ainda neste módulo desta disciplina), que atualmente, com desenvolvimento e aprimoramento aplicados à elas, têm oferecido maiores recursos aos desenvolvedores de jogos e demais profissionais da área gráfica.

Veremos um pequeno exemplo de uso da biblioteca OpenGL e seus comandos? Então nos acompanhe!


Exemplo de arquivo em C++ apenas para visualização do uso da OpenGL:

//Interliga o código com a biblioteca glut
#include <glut.h>

void abreJanela() {
// Limpa o buffer de pixels
glClear(GL_COLOR_BUFFER_BIT);
// Executa os comandos OpenGL
glFlush();
}

int main(int argc, char* argv[]) {
// Inicia a biblioteca Glut
glutInit(&argc, argv);
// Define o tipo do modo de exibição e formato de cores
glutInitDisplayMode(GLUT_SINGLE | GLUT_RGBA);
// Define o tamanho da tela
glutInitWindowSize(640, 480);
// Cria a tela com o nome inserido no parâmetro
glutCreateWindow(“Minha primeira tela em OpenGL”);
// Define a cor preta para a tela
glClearColor(0, 0, 0, 0);
// Chama a função abreJanela
glutDisplayFunc(abreJanela);
// Inicia a execução dos recursos
glutMainLoop();
// Valor de retorno
return 0;
}


Agora, apresentaremos um exemplo de utilização de biblioteca de função. Acompanhe o passo-a-passo que exibiremos a seguir!



Exemplo de aplicação de bibliotecas de função
O surgimento deste tipo de biblioteca teve como objetivo principal a simplicidade e o desejo de facilitar o trabalho dos desenvolvedores de aplicações, pois os mesmo iriam necessitar criar inúmeras linhas de código para obter mais um determinado efeito, ou efetuar uma requisição. Com a biblioteca jQuery esse processo é obtido através de poucas instruções, fazendo com que a jQuery se transformasse em uma ferramenta ideal para os projetistas de sites e desenvolvedores que possuíssem conhecimento limitado em JavaScript.

E aí, estudante, vamos ao exemplo de utilização dela? Vamos lá!


Exemplo de arquivo HTML+JavaScript apenas para visualização do uso da jQuery:

<!DOCTYPE html>
<html>
<head>
<script src=”/lib/jquery-1.12.2.min.js”></script> (aqui ligamos com a biblioteca)
<script>
$(document).ready(function(){
$(“button”).click(function(){
$(“div”).animate({
height: ‘toggle’
});
});
});
</script>
</head>
<body>
<p>Para abrir e fechar o quadro, clique no botão.</p>
<button>Animar</button>
<div style=”background:#FF0000;height:100px;width:100px;position:absolute;”></div>
</body>
</html>
Observação: no exemplo acima, a linha onde é feita a referência à biblioteca jQuery mostra o diretório onde os arquivos foram instalados, ou seja, no diretório Lib.

Não se preocupe se você não entendeu os exemplos de códigos apresentados acima, pois a intenção era somente dar uma ideia de como os dois tipos de bibliotecas se interligam aos códigos. Logo, teremos a oportunidade de nos aprofundarmos neste assunto.


