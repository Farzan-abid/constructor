# constructor
a simple  C++ code working on class and constructor for OOps
 #include <iostream>
 #include <string>
 #include<list>
 #include <cstdlib>
 using namespace std;
 class youtubechannels{
 	public:
 	string name;
 	string ownername; 
 	int subscribers;
 	list<string> publishedtitles;

 	
 	youtubechannels(string Name,string Ownername){
 	name=Name;
 	 ownername=Ownername;
 	subscribers=0;	
	 }
	 
	 void getinfo(){
	 	cout<<" NAME :"<<name<<endl;
	 	cout<<" OWNER NAME :"<<ownername<<endl;
	 	cout<<" SUBSCRIBERS :"<<subscribers<<endl;
	 	cout<<" VIDEOS :"<<endl;
	 	for(string title:publishedtitles){
	 		cout<<title<<endl;
		 }
	 }
 	
 };
 int main(){
youtubechannels ytchannel1("acousticstudio","Farzan"),ytchannels2("amysings","Amy");
ytchannel1.getinfo();
cout<<endl;
ytchannels2.getinfo();

 	return 0;
 }
 
