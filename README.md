# Project-1-2d-Array-Calculator
# include <iostream>
  
 using namespace std;
 
 int main()
 {
  int s[2][2];
  int i, j;
  cout << "\n2D Array Input:\n";
  for(i=0; i<2; i++)
  {
    for(j=0; j<2; j++)
    {
      cout << "\ns[" <<i<< "]["<<j<<"]= ";
      cin >> s[i][j];
    }
  }
  
  cout << "\n The 2-D Array is: \n";
  for(i=0; i<2; i++)
  {
    for(j=0; j<2; j++)
    {
      cout << "\t" <<s[i][j];
    }
    cout << endl;
   }
}
 
 int main()
 {
    char op;
    float num1, num2;
    
    cout << "Enter operator either +, -, * or /: ";
    cin >> op;
    
    cout << "Enter two operands: ";
    cin >> num1 >> num2;
    
    switch(op)
    {
      case '+':
        cout << num1+num2;
        break;
        
      case '-':
        cout << num1-num2;
        break;
        
      case '*':
        cout << num1*num2;
        break;
        
      case '/':
        cout << num1/num2;
        break;
 }
 
 return 0;
