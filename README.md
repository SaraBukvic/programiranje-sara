# programiranje-sara
zadaci
 #include<iostream>
#include<string>
using namespace std;

void gime(string ime, string prezime, string djevprez, string gradr){


string fname,bcity,swname;
fname=ime.substr(0,3);
bcity=gradr.substr(0,2);
swname=fname+bcity;

string surname, gradrod, swsurname;
surname=djevprez.substr(0,2);
gradrod=gradr.substr(0,3);
swsurname=surname+gradrod;
cout<<"Vase StarWars ime je:"<<swname<<" "<<swsurname<<endl;
}
int main()
{

  string ime,prezime,djevprez,gradr;
  cout<<"Unesite ime:"<<endl;
  cin>>ime;
  cout<<"Unesite prezime:"<<endl;
  cin>>prezime;
  cout<<"Unesite djevojacko prezime majke:"<<endl;
  cin>>djevprez;
  cout<<"Unesite grad u kojem ste rodjeni:"<<endl;
  cin>>gradr;
  cout<<endl;
  gime(ime, prezime, djevprez, gradr);
}

2. #include<iostream>
using namespace std;
void racFunkcije(int x, int y)
{
  int r, br;
  br=0;
  for(int i=x;i<y+1;i++){
    br+=1;
    r=i*i+2*i-5;
    cout<<"Rjesenje ["<<br<<"] broj gdje je vrijednost X["<<i<<"] = "<<r<<endl;
  }
}
int main()
{

  int x, y;
  unesi:
  cout<<"Unesite pocetak opsega: "<<endl;
  cin>>x;
  cout<<"Unesite kraj opsega: "<<endl;
  cin>>y;
  if(x>y || x==y){
    cout<<"Pocetak ne moze bit manji od kraja opsega. Unesite ponovo!"<<endl;
    cout<<endl;
 
    goto unesi;
  }
  else{
    racFunkcije(x,y);
  }
return 0;
}
