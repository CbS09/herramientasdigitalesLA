# herramientasdigitalesLA
Ejercicios en clase 

//Hola Andrés, esto lo hice en processing, enjoy!

//espejo y blanco es X y zancudo y chao es Y
//Triángulo superior
 int espejo = 10;
 int zancudo = 35;

//Triángulo inferior
public int blanco = 500;
public int chao = 550;

//para definir el tamaño del canvas
void setup () {
     size (960, 540);   
//color de fondo     
     background (150,150,255);
}

//para definir lo que está adentro del canvas
void draw () {
  // para obtener distintas gamas de color se utiliza random en fill
 fill (random (0, 150), 150, 50); 
 ellipse(480, 260, 20, 20);
 
 //la ubicación de las figuras es de adentro para afuera
   
 fill (255, 255, 255);
 ellipse(460, 260, 10, 10);
 ellipse(500, 260, 10, 10);
 ellipse(480, 280, 10, 10);
 ellipse(480, 240, 10, 10);
 
 fill (200, 125, 125);
 ellipse(500, 245, 20, 10);
 ellipse(500, 275, 20, 10);
 ellipse(460, 275, 20, 10);
 ellipse(460, 245, 20, 10);
 
 //para obtener color transparecia se pone un cuarto número en fill
 fill (200, 125, 125,0);
 //para cambiar el color de los bordes
 stroke (50,150, 200);
 ellipse(480, 220, 70, 70);
 ellipse(480, 300, 70, 70);
 ellipse(520, 260, 70, 70);
 ellipse(440, 260, 70, 70);
 
 fill (250, 250, 125);
 ellipse(480, 310, 25, 25);
 ellipse(480, 210, 25, 25);
 
 fill (250, 90, 120);
 ellipse(530, 260, 25, 25);
 ellipse(435, 260, 25, 25);
 
 fill (0, 150, 150, 50);
 ellipse(435, 205, 10, 30);
 ellipse(435, 315, 10, 30);
 ellipse(525, 315, 10, 30);
 ellipse(525, 205, 10, 30);
 
 fill (20, 250, 150, 50);
 ellipse(390, 260, 20, 20);
 ellipse(570, 260, 20, 20);
 ellipse(480, 350, 20, 20);
 ellipse(480, 170, 20, 20);
 
 fill (20, 200, 200, 50);
 ellipse(505, 180, 15, 15);
 ellipse(455, 180, 15, 15);
 ellipse(455, 340, 15, 15);
 ellipse(505, 342, 15, 15);
 
 fill (200, 250, 150, 50);
 ellipse(480, 220, 55, 25);
 ellipse(480, 300, 50, 25);
 
 fill (20, 80, 150, 50);
 ellipse(550, 310, 10, 10);
 ellipse(410, 310, 10, 10);
 ellipse(410, 220, 10, 10);
 ellipse(550, 220, 10, 10);
 
 fill (200, 80, 150,0);
 stroke (150,150, 200,20);
 ellipse(570, 260, 70, 50);
 ellipse(400, 260, 70, 50);
 
 fill (20, 280, 50,0);
 stroke (250,250, 80,20);
 ellipse(555, 310, 40, 40);
 ellipse(555, 215, 40, 40);
 ellipse(405, 212, 40, 40);
 ellipse(405, 310, 40, 40);
 
 stroke (50,150, 200);
 fill (200, 200, 250);
 ellipse(340, 260, 70, 10);
 ellipse(620, 260, 70, 10);
 
 fill (110, 150, 150);
 ellipse(480, 380, 15, 15);
 ellipse(480, 140, 15, 15);
 
 stroke (150,150, 200,20);
 fill (200, 200, 250,0);
 ellipse(480, 410, 30, 90);
 ellipse(480, 110, 30, 90);

//para poner texto se utliza text
 String s = "por Camila Barajas Salej";
 textSize(20);
 fill(255, 255, 255);
 text(s, 680, 500);
 
 // fin de los círculos inicio otras figuras
 fill(50,0 , 100);
 stroke (0,20,255);
 espejo = espejo + 10;
 //triángulo superior
 triangle (espejo, zancudo, 30, 0, 56, zancudo);
 
if (espejo > width){
   espejo=0;
   zancudo= zancudo+50;
    }
//triangle (x1, y1, x2 (punta), y2, x3, y3);
  blanco = blanco + 10;
  //triángulo inferior
  triangle (600, chao,990, blanco, 990, chao);
  
if (blanco > width){
   blanco=0;
   chao= chao+10;
    }  
 
}
