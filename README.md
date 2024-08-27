# Implementation_Of_Custom_STRING_Class_In_CPP
# Overview
This project "Implementation Of Custom STRING Class" is implemented to create our custom STRING class which will have the same functionality as the existing string class.
- The STRING class has the following basic functionalities: 
  + Constructor with no arguments
  + Parameterised Constructor with only one argument
  + Copy Constructor
  + Destructor
- Some more functionalities of STRING class are mentioned below in features...
  
# Main Menu
Created a executable file named "string" from different modules like main.cpp,memb_fn_defns.cpp,friend_fns.cpp....etc.., when executed will perform the main program accordingly.
# Features
## Below main code has all the functionalities of STRING class that are included in this project:
#include"header.h"

int main()

{
	
 int i;
	
 STRING s1;
	
 cout<<"Enter str:"<<endl;
	
 cin>>s1; 
	
 STRING s2 = s1;
	
 cout<<"\ns1: "<<s1<<endl;
	
 cout<<"s2=s1: "<<s2<<endl<<endl;
	
 STRING s3 = s1+s2, s4("Vector");
	
 cout<<"s3 = s1+s2: "<<s3<<endl;
	
 s3 = s1+s2+s3;
	
 cout<<"s3 = s1+s2+s3: "<<s3<<endl;
	
 cout<<endl<<"s4(""Vector"") : "<<s4<<endl;
	
 STRING s[5]={"Hii","boy"};
	
 cout<<"\nArray as s[5]={""Hii"",""boy""}\n"<<"s[0]: "<<s[0]<<endl<<"s[1]: "<<s[1]<<endl;
	
 cout<<"Enter s[2]:"<<endl;
	
 cin>>s[2];
	
 s[3] = "India";
	
 s[4] = s[3] + s4;
	
 cout<<"\nArray ele:\n";
	
 for(i=0; i<5; i++)
		
  cout<<s[i]<<endl;
	
 if(s1 == s2)
		
  cout<<"\ns1 == s2"<<endl;
	
 else
		
  cout<<"\ns1 != s2"<<endl;	
	
 if(s[3] != s[4])
		
  cout<<"\ns[3] != s[4]"<<endl<<"India != VectorIndia"<<endl;
	
 else
		
  cout<<"\ns[3] == s[4]"<<endl<<"India == VectorIndia"<<endl;
	
 if(s[3] > s[4])
		
  cout<<"\ns[3] > s[4]"<<endl<<"India > VectorIndia"<<endl;
	
 else
		
  cout<<"\ns[3] > s[4] is false"<<endl<<"India > VectorIndia is false"<<endl;
		
	
 if(s[3] < s[4])
		
  cout<<"\ns[3] < s[4]"<<endl<<"India < VectorIndia"<<endl;
	
	
 s[4] = s[3];
	
 cout<<"\ns[4]=s[3]: "<<s[4]<<endl;

	
 if(s[3] >= s[4])
		
  cout<<"\ns[3] >= s[4]"<<endl<<"India >= India"<<endl;			
	
 if(s[3] <= s[4])
		
  cout<<"\ns[3] <= s[4]"<<endl<<"India <= India"<<endl;
	

	
 STRncpy(s[4],s[3],3); //Ind India
	
 cout<<STRcmp(s2,s4)<<endl;
	
 cout<<STRncmp(s[4],s[3],6)<<endl; 
 
	
 STRcat(s[0],s[1]);
	
 STRncat(s[1],s[2],2);
	
 STRrev(s[4]);
	
 STRupper(s[4]);
	
 STRlower(s[4]);
	
	
 cout<<"\nAfter array ele:\n";
	
 for(i=0; i<5; i++)
		
  cout<<s[i]<<endl;

	
 cout<<STRchr(s[4],'a')<<endl;
	
 cout<<STRrchr(s[4],'a')<<endl;
	
 cout<<STRlen(s[4])<<endl;
	
 STRING s5 = "dni";
	
 cout<<STRstr(s[4],s5)<<endl;

}
















