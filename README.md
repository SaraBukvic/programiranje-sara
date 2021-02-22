# programiranje-sara
zadaci
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
