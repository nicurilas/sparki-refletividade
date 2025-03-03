# sparki-refletividade
Este código foi desenvolvido para ser executado no Sparki, robô educacional e programável da Edubot. 
Funcionalidade
O código faz o seguinte:
1.	Mede a refletividade da superfície sob o robô em cinco pontos diferentes;
2.	Calcula a média dessas medições;
3.	Exibe o valor médio no display LCD do robô.
________________________________________
Variáveis
•	refl1, refl2, refl3, refl4, refl5: Armazenam os valores de refletividade medidos em cinco pontos distintos.
•	media: Armazena a média dos cinco valores de refletividade.
________________________________________
Funções e Métodos
•	sparki.lineCenter(): Mede a refletividade da superfície sob o robô. Retorna um valor que representa a intensidade da luz refletida (geralmente entre 0 e 1000, onde 0 é totalmente preto e 1000 é totalmente branco).
•	sparki.moveForward(1): Faz o robô avançar uma pequena distância (1 cm neste caso).
•	sparki.clearLCD(): Limpa o display LCD do robô.
•	sparki.print(media): Exibe o valor da média no display LCD.
•	sparki.updateLCD(): Atualiza o display LCD para mostrar as alterações.
•	delay(): Pausa a execução do programa por um número específico de milissegundos.
________________________________________
Fluxo do Programa
1.	Inicialização (setup):
o	O bloco setup() está vazio, o que significa que nenhuma configuração inicial é realizada antes do início do loop principal.
2.	Loop:
o	O robô mede a refletividade no ponto atual (refl1) e aguarda 300 ms.
o	Em seguida, avança 1 cm e mede a refletividade no novo ponto (refl2), aguardando outros 300 ms.
o	Esse processo é repetido para refl3, refl4 e refl5, avançando 1 cm entre cada medição.
o	Após as cinco medições, calcula a média dos valores de refletividade e armazena na variável media.
o	Limpa o display LCD, exibe o valor da média e atualiza o display.
o	Por fim, aguarda 3 segundos antes de repetir o loop.
________________________________________

