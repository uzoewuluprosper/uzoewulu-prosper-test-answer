struct Node
{ float Number ;
Node *Link ;
} ;
class STACK
{ Node *Top ;
public :
STACK( ) {Top = NULL ;}
void PUSH( ) ;
void POP( ) ;
~STACK( ) ;
} ;
void STACK::PUSH( )
{ Node *Temp;
Temp=new Node;
if(Temp= =NULL)
{
cout<<”\nNo memory to create the node…”;
exit(1);
}
cout<<”\nEnter the Number to be inserted: “;
cin>>Temp→ Number;
Temp→ Link=Top;
Top=Temp;
}

