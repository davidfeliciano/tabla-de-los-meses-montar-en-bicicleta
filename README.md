# tabla-de-los-meses-montar-en-bicicleta

// variable fuente y la nombro .:::::
PFont gluck;

//llamar la fuente en herramientas-traer fuente etc el mismo tamaño del que voy a dejar el texto 
String monate []= {"Enero","Febrero","Marzo","Abril","Mayo","Junio","Julio","Agosto","Septiembre",
"Octubre","Noviembre","Vacaciones"};
//

   int jahr[] ={100,200,300,350,101,200,
   305,200,300,400,300,302
 };
    int compras[] ={3,5,10,7,10,2,
   15,3,10,25,25,25
 };
 
 
 void setup(){
  size(1080,720);
  gluck = loadFont("Aparajita-Bold-20.vlw");

  textFont(gluck,20);

smooth(5);
}

void draw(){
  background(235);
  text("MONO",1020,720);
 
                       

  for(int equis = 0; equis< 12; equis=equis+1){
    if(jahr[equis]>115){
      fill(0,250,0);}else {fill(#CB4646);}
  text(monate[equis],50,20+(equis*60));
  rect(200,(equis*60),jahr[equis],10);
  text(jahr[equis],215+jahr[equis],30+(equis*60));
  
  for(int anu = 0; anu< 12; anu=anu+1){
    if(compras[anu]>115){
      fill(0,250,0);}else {fill(#CB4646);}
  text(monate[anu],50,20+(anu*60));
  rect(200,(anu*60),compras[anu],20);
  text(compras[anu],215+compras[anu],30+(anu*60));
  }
}
}
