import 'dart:io';

void main() {
  print ("Bem-vindo ao gerador de código da App Store! ");
  print ("Vamos gerar um código exclusivo para você! ");

  //Solicita ao usuário a quantidade de códigos que deseja gerar
  print("Digite a quantidade de códigos que deseja gerar: ");
  var qty = stdin.readLineSync();
  int qtyInt = int.parse(qty);

  //Cria um loop para gerar a quantidade de códigos especificada
  for (int i = 0; i < qtyInt; i++){
    //Gera um número aleatório entre 0000 e 9999
    int codeNum = (Random().nextInt(9999 - 0000 + 1) + 0000);

    //Imprime o código criado na tela
    print("Seu código gerado é: ");
    print("+ 7 $codeNum");
  }
  
  print ("Gerando códigos concluídos! ");
  
}
