float X;
float Y;
float sudut;
float skala;

// Membuat Setup-nya terlebih dahulu
void setup(){
 size (1000, 800);
 X = width / 2; 
 Y = height / 2;
 sudut = 0;
 skala  = 1.0;
}

// Menggambar objek 2D sekaligus memasukkan fungsi yang diperlukan
void draw(){
 background(#D707E3);
 
 pushMatrix();
 translate(X, Y);
 rotate(radians(sudut));
 scale(skala);
 drawMNA();
 popMatrix();
 if (keyPressed){
   if(keyCode == UP){
     Y -= 2;
  }else if (keyCode == DOWN){
     Y += 2;
  }else if (keyCode == LEFT){
     X -= 2;
  }else if (keyCode == RIGHT){
     X += 2;
 }
 }
}

// Fungsi agar keyboard dapat berinteraksi dengan fungsi rotate dan ZoomIn/Out
void keyPressed(){
  if (key == 'w'){
    skala += 0.1;
  }else if(key == 'a'){
    sudut += 5;
  }else if(key == 's'){
    skala -= 0.1;
  }else if(key == 'd'){
    sudut -= 5;
}
}

//Contoh objek 2D yang akan digerakkan berupa teks "MNA"
void drawMNA(){
  textSize(60);
  textAlign(CENTER, CENTER);
  fill(0);
  text("MNA", 0, 0);
}
