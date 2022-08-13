# Bandeira do Brasil

<!DOCTYPE html>
<meta charset="UTF-8">

<!-- bandeira-brasil.html -->
<center>
<canvas width="600" height="400" id=”brasil”></canvas>

<h3>BADEIRA DO BRASIL EM JAVASCRIPT</h3>

  
<script>
	
	

   var tela = document.querySelector('canvas');
   var pincel = tela.getContext('2d');
       p = pincel;

   document.write("By Gilmario Santos");

    // codigo para desenha o retangulo  verde
    p.fillStyle='green';
    p.fillRect(0, 0, 600, 400);
    // fim do codigo 

    // codigo do losango 
    p.fillStyle='yellow';
    p.beginPath();
    p.moveTo(300, 50);
    p.lineTo(50, 200);
    p.lineTo(550, 200);
    p.fill();
    // fim do codigo

    
    // codigo do circulo azul 
    p.beginPath();
    p.moveTo(300, 350);
    p.lineTo(50, 200);
    p.lineTo(550, 200);
    p.fill();
    p.fillStyle='darkblue';
    p.beginPath();
    p.arc(300, 200, 100, 0, 2*3.14);
    p.fill();
    // fim do codigo
   

    // codigo para desenha a faixa do centro do circulo
    p.fillStyle='#FFFFFF';
    p.beginPath();
    p.arc(290, 275, 120, 10,2*3.0);
    p.fill();
    p.fillStyle='darkblue';
    p.beginPath();
    p.arc(289, 285, 110, 10,2*3.-0);
    p.fill();
    // fim do codigo
 

     // Posição das estrelas na bandeira
     p.font = '15px arial black';
     p.strokeStyle='yellow'//#FFFFFF'
     p.strokeText('☆', 330, 158); 
     p.font = '10px arial black';
     p.strokeText('☆', 215, 220); 
     p.strokeText('☆', 257, 200); 
     p.font = '5px arial black';
     p.strokeText('☆', 252, 223); 
     p.font = '10px arial black';
     p.strokeText('☆', 242, 240);
     p.font = '8px arial black';
     p.strokeText('☆', 230, 252); 
     p.font = '10px arial black';
     p.strokeText('☆', 280, 270); 
     p.font = '5px arial black';
     p.strokeText('☆', 270, 250); 
     p.font = '8px arial black';
     p.strokeText('☆', 265, 235); 
     p.font = '8px arial black';
     p.strokeText('☆', 330, 200);
     // cruzeiro do sul
     p.font = '9px arial black';
     p.strokeText('☆', 300, 220);
     p.font = '7px arial black';
     p.strokeText('☆', 290, 230);
     p.font = '5px arial black';
     p.strokeText('☆', 315, 225);
     p.strokeText('☆', 300, 235);
     p.font = '9px arial black';
     p.strokeText('☆', 305, 250);
     // fim do cruzeiro do sul
     p.font = '3px arial black';
     p.strokeText('☆', 320, 270);
     p.font = '8px arial black';
     p.strokeText('☆', 360, 230);
     p.font = '5px arial black';
     p.strokeText('☆', 373, 230);
     p.strokeText('☆', 350, 240);
     p.font = '8px arial black';
     p.strokeText('☆', 330, 252);
     p.font = '7px arial black';
     p.strokeText('☆', 340, 265);
     // fim parte das estrelas 

     // circulo para corrigir borda da faixa
     p.beginPath();
     p.arc(300, 200, 100, 0, 2*Math.PI);
     p.lineWidth = 20;
     p.stroke();
     // fim do codigo

     // codigo para colocar texto em forma de arco na bandeira   
     p.font = "14px arial black";
     p.fillStyle = "green";
     
     let string = "ORDEM E PROGRESSO";
     let angle = Math.PI * 0.6; 
     let radius = 102;
    
     p.translate(290, 271);
     p.rotate(-2 * angle / 4);

     for (let i = 0; i < string.length; i++) {
     	p.rotate(angle / string.length);
        p.save();
        p.translate(0, -1 * radius);
        p.fillText(string[i], 0, 0);
        p.restore();
      }
      // fim do codigo

   
</script>
</center>
